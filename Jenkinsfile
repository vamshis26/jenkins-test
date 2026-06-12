pipeline {
    agent any

    tools {
        nodejs 'NodeJS'
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Run JavaScript') {
            steps {
                sh 'node test.js'
            }
        }
    }
}
