pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }

        stage('Check Node & npm') {
            steps {
                sh 'node -v'
                sh 'npm -v'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run JavaScript File') {
            steps {
                sh 'node test.js'
            }
        }

    }

    post {
        success {
            echo 'Build completed successfully 🎉'
        }

        failure {
            echo 'Build failed ❌'
        }
    }
}
