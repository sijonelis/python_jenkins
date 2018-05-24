pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                    docker {
                        image 'python:2-alpine' 
                    }
                }
           try {

                sh "docker run -e python:2-alpine"
           } catch (error) {

           } finally {

           }

        }

    stage('Run Tests') {
        try {
            sh 'python --version'
          //dir('webapp') {
          //  sh "mvn test"
          //  docker.build("arungupta/docker-jenkins-pipeline:${env.BUILD_NUMBER}").push()
          //}
        } catch (error) {

        } finally {
          //junit '**/target/surefire-reports/*.xml'
        }
      }
    }
}