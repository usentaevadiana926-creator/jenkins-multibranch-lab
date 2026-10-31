pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code is available'
            }
        }

        stage('Build') {
            steps {
                echo 'Updated feature-demo branch for Task 9'
            }
        }

        stage('Test') {
            steps {
                sh 'python3 -m pytest -v'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }

        failure {
            echo 'Pipeline failed. Check the logs'
        }
    }
}