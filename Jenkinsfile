pipeline {
    agent any
    
    stages {
        stage('Build Docker image') {
            steps {
                sh 'docker build -t user-java .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run -dp 3000:3000 user-java'
            }
          }
    }
}
