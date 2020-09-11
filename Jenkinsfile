pipeline {
    agent {dockerfile true}
    
    environment{
    R_LIBS_SITE='/usr/local/lib/R/site-library:/usr/lib/R/site-library:/usr/lib/R/library:'
    }
    
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
                sh 'R -e "Sys.getenv()"'
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
