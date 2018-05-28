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
    }
}
