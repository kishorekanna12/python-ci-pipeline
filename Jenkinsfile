pipeline {
    agent any

    stages {
        // Stage 1: Checkout Code
        stage('Checkout Code') {
            steps {
                echo 'Stage 1: Pulling latest code from GitHub...'
                checkout scm
            }
        }

        // Stage 2: Build
        stage('Build') {
            steps {
                echo 'Stage 2: Verifying and executing the Python program...'
                bat 'python sum_app.py' //  This works perfectly on Windows
            }
        }
    }
}
