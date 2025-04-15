pipeline {
    agent any

    environment {
        APP_NAME = "zigbato-food-delivery-app"
    }

    stages {
        stage('Checkout') {
            steps {
                // This will use the repository specified in the job configuration
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building the Zigbato app...'
                // Replace these commands with your actual build commands
                // Example for Node.js:
                // sh 'npm install'
                // sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Insert your test commands here
                // Example: sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the Zigbato app...'
                // Insert your deployment commands here
                // For example: copy files or run a deployment script
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Please review the logs.'
        }
    }
}
