pipeline {
    agent any

    stages {

        stage('Debug Workspace') {
            steps {
                sh 'pwd'
                sh 'ls -la'
            }
        }

        stage('Check Node') {
            steps {
                sh 'node -v'
                sh 'npm -v'
            }
        }

        stage('Run JS') {
            steps {
                sh 'node test.js'
            }
        }
    }
}
