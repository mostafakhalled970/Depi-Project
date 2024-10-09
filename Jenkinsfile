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
                sh 'echo Running tests...'
            }
        }
    }
}

