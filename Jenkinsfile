pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building the project..."'
                sh './gradlew build' // replace with your build command
            }
        }
        stage('Test') {
            steps {
                sh './gradlew test' // replace with your test command
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying the project..."'
                // add your deployment steps here
            }
        }
    }
}
