pipeline {
    agent any
    
    tools {
        maven 'M3'
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('mvn-build') {
            steps {
                script{
                    sh "mvn clean install"
                }
            }
        }
    }
}
