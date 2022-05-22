pipeline {
    agent {
        docker {
            image 'node:12-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Testing') { 
            steps {
                sh 'node -v'
                sh 'npm -v' 
            }
        }
    }
}