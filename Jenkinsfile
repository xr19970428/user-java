pipeline {
    agent any
    
    stages {
        stage('Build Docker image') {
            steps {
                sh 'docker build -t openhack-devops-team/apis/user-java .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh 'docker run -dp 3000:3000 openhack-devops-team/apis/user-java'
            }
          }
    }
}
