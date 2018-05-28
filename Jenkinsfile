pipeline {
    agent none
    stages {
        stage('docker') {
            agent any
            steps {
                sh 'docker --version'
                sh 'docker images'
            }
        }
        stage('mvn') {
            agent { docker 'maven:3.3.3' }
            steps {
                sh 'docker-compose up'
            }
        }
    }
}
