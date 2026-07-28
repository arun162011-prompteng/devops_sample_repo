pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'py -3.10 -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'py -3.10 -m pytest -v'
            }
        }
    }
}