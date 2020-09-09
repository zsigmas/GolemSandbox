pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'make build'
            }
        }
        stage('Check') {
            steps {
                echo 'Checking...'
            }
        }
        stage('Clean') {
            steps {
                echo 'Cleaning...'
            }
        }
    }
}
