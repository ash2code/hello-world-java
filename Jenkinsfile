pipeline {
    agent any
    
    tools {
        maven 'M3'
    }

    stages {
        stage('git-checkout') {
            steps {
                script {
                    git 'https://github.com/ash2code/hello-world-java.git/'
                }
            }
        }
        stage('mvn-build') {
            steps {
                script {
                    sh "mvn clean install"
                }
            }
        }
    }
}
