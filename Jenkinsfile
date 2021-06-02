pipeline {
    agent any
    stages {
        stage("SetupVirtualEnv") {
            steps {
                withPythonEnv("/usr/bin/python3") {
                    sh 'pip install -r requirements.txt'

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
