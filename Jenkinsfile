pipeline {
    agent any

    stages {
        stage('Verify Python') {
            steps {
                bat 'python --version'
                bat 'python -m pip --version'
                bat 'where python'
            }
        }
    }
}