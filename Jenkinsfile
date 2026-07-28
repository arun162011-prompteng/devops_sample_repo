pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'python -m pip install -r requirements.txt'
            }
        }

        stage('Run Unit Tests') {
            steps {
                bat 'python -m pytest -v'
            }
        }

    }

    post {
        success {
            echo 'CI Pipeline completed successfully!'
        }

        failure {
            echo 'CI Pipeline failed.'
        }
    }
}