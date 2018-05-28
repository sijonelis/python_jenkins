pipeline {
    agent { 
        docker 'maven:3-alpine' 
        args { -v /var/run/docker.sock:/var/run/docker.sock}
    } 
    stages {
        stage('Example Build') {
            steps {
                sh 'mvn -B clean verify'
            }
        }
    }
}