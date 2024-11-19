pipeline {
    agent {
        docker { image 'node:14' } // Pulls and uses the Node.js 14 Docker image
    }
    stages {
        stage('Checkout') {
            steps {
                // Fetches the code from your GitHub repository
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh 'node --version' // Verifies the Node.js version inside the container
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests ..."' // Placeholder for actual test commands
            }
        }
    }
    post {
        success {
            echo 'Build and Test succeeded!' // Logs a success message
        }
        failure {
            echo 'Build or Test failed!' // Logs a failure message
        }
    }
}
