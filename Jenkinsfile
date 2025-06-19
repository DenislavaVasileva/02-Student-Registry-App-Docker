pipeline {
    agent any

    stages {
        stage('Checkout the repo') {
            steps {
                checkout scm
            }
        }

        stage('Install dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm run test'
            }
        }
    }
}