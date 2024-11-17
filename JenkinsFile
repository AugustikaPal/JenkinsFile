pipeline {
    agent {
        docker { image 'node:14' } // Pulls and uses the Node.js 14 Docker image
    }
    stages {
        stage('Build') {
            steps {
                sh 'node --version' // Verifies the Node.js version inside the container
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }
    }
}
