pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                
                bat 'wsl ./jenkins/scripts/test.sh'
            }
        }
    }
}