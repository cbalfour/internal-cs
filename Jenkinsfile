pipeline {
    agent any
    stages {
        stage("SetupVirtualEnv") {
            steps {
                withPythonEnv("/usr/bin/python3") {
                    sh 'pip install sphinx'
                }
            }
        }
	stage("Build") {
            steps {
                withPythinEnv("/usr/bin/python3") {
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
