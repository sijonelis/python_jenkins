pipeline {
    agent {
        docker {
            image 'python:2-alpine' 
        }
    }
    stages {
        stage('Setup') { 
            steps {
                sh 'python --version' 
            }
        }
    }
}