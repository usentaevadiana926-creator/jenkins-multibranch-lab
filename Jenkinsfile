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
                echo 'Preparing project'
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