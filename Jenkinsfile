pipeline {
    agent any
    stages {
        stage("SetupVirtualEnv") {
            steps {
                withPythonEnv("/usr/bin/python2.7") {
                    sh 'pip install sphinx'
                }
            }
        }
	stage("Build") {
            steps {
                withPythonEnv("/usr/bin/python2.7") {
                    sh 'make html'
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
