pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/Elics21/rgr.git'
            }
        }

        stage('Build') {
            steps {
                sh 'docker build -t app .'
            }
        }
    }
}
