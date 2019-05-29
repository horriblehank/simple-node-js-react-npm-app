pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }

        stage('Build Production Files') {
            steps {
                bat 'npm run build'
            }
        }

        stage('Echo out') {
            steps {
                bat 'npm run lintme'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}