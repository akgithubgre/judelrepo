pipeline {
    agent any

    stages {
        stage('Pull & Run Custom Docker Image') {
            steps {
                bat 'docker pull akgreninja/node-custom:16-alpine'
                bat 'docker run --rm akgreninja/node-custom:16-alpine node --version'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}
