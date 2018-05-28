pipeline {
    agent none
    stages {s
        stage('docker') {
            agent any
            steps {
                sh 'docker --version'
                sh 'docker images'
            }
        }
    }
}
