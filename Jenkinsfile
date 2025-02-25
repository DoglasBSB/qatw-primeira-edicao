pipeline {
    agent any

    stages {
        stage('Node.js Deps') {
            steps {
                sh 'npm install'
            }
        }
        stage('E2E Testes') {
            steps {
                sh 'npm run play:test '
            }
        }
    }
}
