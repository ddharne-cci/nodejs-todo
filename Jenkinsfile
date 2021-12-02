pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
               git 'https://github.com/ddharne-cci/nodejs-todo.git'
        }
        }
        stage('docker-compose') {
            steps {
                
              sh 'sudo group add docker'
              sh 'sudo usermod -aG docker $USER'
              sh 'chmod 777 /var/run/docker.sock'  
              sh 'docker-compose up --build'
            }
            }
        }
    
        }
