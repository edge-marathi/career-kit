pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Code checkout done!'
                echo "Branch: ${env.GIT_BRANCH}"
            }
        }
        stage('Build') {
            steps {
                echo 'Building application...'
                bat 'echo Build successful'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo All tests passed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                bat 'echo Deployed successfully'
            }
        }
    }
    post {
        success {
            echo 'Pipeline SUCCESS! Omkar rocks!'
        }
        failure {
            echo 'Pipeline FAILED!'
        }
    }
}
