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
                // Your actual test command here
            }
        }
        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                echo 'Deploying...'
                // Your deployment commands here
            }
        }
    }
}

