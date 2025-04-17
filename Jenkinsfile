pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                bat 'docker build -t java-hello-pipeline .'
            }
        }
        stage('Run Docker Container') {
            steps {
                bat 'docker run --rm java-hello-pipeline'
            }
        }
    }
}
