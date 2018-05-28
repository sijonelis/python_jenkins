pipeline {
    agent {
        any
    }
    stages {
        stage('Setup') { 
            agent {
                docker {
                    image 'python:2-alpine' 
                    reuseNode true  
                }
            }
            steps {
                sh 'python --version' 
            }
        }
    }
}