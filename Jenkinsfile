pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/sasidharkk/nodejs-demo-app.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the app...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the app...'
            }
        }
    }
}

