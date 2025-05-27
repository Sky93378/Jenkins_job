pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                echo 'Cloning Repository...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Example for Node.js
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example for Node.js
                bat 'npm test'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}
