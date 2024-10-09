pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    docker.build('app-image')
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Run the tests
                    sh 'pytest tests/'  // Adjust based on your testing framework and directory
                }
            }
        }
        stage('Deploy') {
            steps {
                // Add deployment steps here
            }
        }
    }
}

