pipeline {
    agent none 
        stages {
        ws("/var/jenkins_workspaces/helloworld"){
            stage('Build') { 
                agent {
                    docker {
                        image 'python:2-alpine' 
                        inside '-u 0:0'
                    }
                }
                steps {
                    sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
                }
            }
        }
    } 
}