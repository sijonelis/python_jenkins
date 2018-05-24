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
                    sh 'ls -a'
                    sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
                }
            }
        }
    }
}