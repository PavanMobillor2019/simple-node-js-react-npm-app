pipeline {
    agent {
        docker {
            image 'node:lts-bullseye-slim' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'sudo chown -R 1001:1001 "/.npm"'
                sh 'npm install' 
            }
        }
    }
}