pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:2-alpine' 
                    inside '-u 0:0'
                }
            }
            steps {
                ws("/var/jenkins_workspaces/helloworld"){
                    sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
                }
            }
        }
    }
}