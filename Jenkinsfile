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
    
              sh 'docker-compose up --build'
            }
            }
        }
    
        }
