pipeline {
    agent any

    stages {
        stage('Check Node') {
            steps {
                sh 'which node || echo "Node not found"'
                sh 'node -v || echo "Node is not installed"'
                sh 'npm -v || echo "npm is not installed"'
            }
        }
    }
}
