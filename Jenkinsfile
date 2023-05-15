pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                docker build -t biy_daalt .
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}