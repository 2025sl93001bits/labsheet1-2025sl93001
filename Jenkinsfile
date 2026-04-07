pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out code...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage...'
                sh 'ls -la'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh '''
                python3 calculator.py
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage (dummy)...'
                echo 'Application deployed successfully!'
            }
        }
    }
}
