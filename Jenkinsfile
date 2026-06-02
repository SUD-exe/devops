pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
                echo '✅ Repository cloned successfully'
            }
        }

        stage('Build') {
            steps {
                sh 'echo Building application...'
            }
        }

        stage('Test') {
            steps {
                sh 'echo Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo Deploying application...'
            }
        }
    }

    post {
        success {
            echo '🎉 PIPELINE SUCCESS'
        }

        failure {
            echo '🔥 PIPELINE FAILED'
        }
    }
}