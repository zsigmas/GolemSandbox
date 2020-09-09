pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'make build'
            }
        }
        stage('Test') {
            steps {
                echo 'Checking...'
                sh 'make check'
            }
        }
        stage('Clean') {
            steps {
                echo 'Cleaning...'
                sh 'make clean'
            }
        }
    }
}
