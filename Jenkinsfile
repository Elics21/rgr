pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Elics21/rgr.git'
            }
        }

        stage('Build') {
            steps {
                sh 'docker build -t app .'
            }
        }
    }
}
