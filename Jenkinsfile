pipeline {
    agent {
        docker {
                image 'maven:3.3.3'
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
