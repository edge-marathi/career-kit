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
                sh 'echo Build successful'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo All tests passed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'echo Deployed successfully'
            }
        }
    }
    post {
        success {
            echo 'Pipeline SUCCESS!'
        }
        failure {
            echo 'Pipeline FAILED!'
        }
    }
}
