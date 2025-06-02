pipeline{
    agent {
        docker {
            image 'node:18-alpine'  // Uses a Linux Node.js container
            args '-u root'  // Optional: run as root to avoid permission issues
        }
    }
    stages{
        stage('Build') {
            steps{
                sh 'npm install'
            }
        }
        stage('Test'){
            steps{
                sh ' ./jenkins/scripts/test.sh'
            }
        }
    }       
    
}