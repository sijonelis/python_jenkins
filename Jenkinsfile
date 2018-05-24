pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:2-alpine' 
                }
            }
            steps {
                ws("/var/jenkins_workspaces/"){
                    sh 'python --version' 
                }
            }
        }
    }
}