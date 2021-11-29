pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
               git 'https://github.com/ddharne-cci/todo-app.git'
        }
        }
        stage('docker-compose') {
            steps {
                
           
              sh 'docker-compose up --build'
            }
            }
        }
    
        }
