pipeline {
  agent any

  stages {
    stage('Run in Docker') {
      steps {
        bat 'docker pull node:16-alpine'
        bat 'docker run --rm node:16-alpine node --version'
      }
    }
  }
}