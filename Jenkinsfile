pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Elics21/rgr.git'
            }
        }

        stage('Build') {
            steps {
                sh 'docker build -t app .'
            }
        }

        stage('Deploy') {
            steps {
                sh 'docker-compose down && docker-compose up -d'
            }
        }
    }
}
