pipeline {
    agent {
        docker {
                    image 'maven:3.3.3'
                    args '-v /var/jenkins_data:/var/jenkins_data'
                    reuseNode true
            }
    }
    stages {
        stage('docker') {
            agent any
            steps {
                sh 'docker --version'
                sh 'docker images'
            }
        }
        stage('mvn') {
            agent any
            steps {
                sh 'docker-compose up'
            }
        }
    }
}
