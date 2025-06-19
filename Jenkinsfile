pipeline {
    agent any

    stages {
        stage('Checkout the repo') {
            steps {
                checkout scm
            }
        }

        stage('Install dependencies') {
            step {
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            step {
                bat 'npm run test'
            }
        }
    }
}