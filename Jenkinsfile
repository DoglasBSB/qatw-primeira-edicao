pipeline {
    agent {
        dockker {
            image 'mcr.microsoft.com/playwright:v1.50.1-noble',
            args '--network qatw-primeira-edicao_skynet'
        }
    }

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
