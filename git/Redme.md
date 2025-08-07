

pipeline {
    agent any  // Runs on any available Jenkins agent

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Replace with your actual build command
                sh 'echo "Running build command"'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Replace with your actual test command
                sh 'echo "Running test command"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Replace with your deploy command
                sh 'echo "Deploying to environment"'
            }
        }
    }
}
