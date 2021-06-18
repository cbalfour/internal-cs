pipeline {
    agent any
    environment {
        SPHINX_DIR  = '.'
        BUILD_DIR   = './_built'
        SOURCE_DIR  = '.'
        DEPLOY_HOST = 'internal@web0.cs.uct.ac.za:_built'
    }
    stages {
        stage('InstallDependencies') {
            steps {
                sh '''
                    virtualenv venv
                    . venv/bin/activate
                    #pip install -r ${SPHINX_DIR}/requirements.txt
                    pip install sphinx
                '''
            }
        }
        stage('Build') {
            steps {
                sh 'rm -rf ${BUILD_DIR}'
                sh 'rm -f ${SPHINX_DIR}/sphinx-build.log'
                sh '''
                    ${WORKSPACE}/venv/bin/sphinx-build \
                    -q -w ${SPHINX_DIR}/sphinx-build.log \
                    -b html \
                    -d ${BUILD_DIR}/doctrees ${SOURCE_DIR} ${BUILD_DIR}
                '''
            }
            post {
                failure {
                    sh 'cat ${SPHINX_DIR}/sphinx_build.log'
                }
            }
        }
        stage("Archive") {
            steps {
                sh 'zip -r internal.zip ${BUILD_DIR}'
                archiveArtifacts artifacts: 'internal.zip', onlyIfSuccessful: true
            }

        }
        stage("Deploy") {
            steps {
                sshagent(credentials: ['deploy-internal']) {
                    sh '''#!/bin/bash
                        RSYNCOPT=(-aze 'ssh -o StrictHostKeyChecking=no')
                        rsync "${RSYNCOPT[@]}" \
                        --log-file=${SPHINX_DIR}/rsync.log \
                        internal.zip ${DEPLOY_HOST}
                    '''
                }
            }
        }
        stage("HelloWorld") {
            steps {
               sh "echo 'Hello, World!'"
            }
        }
    }
}
