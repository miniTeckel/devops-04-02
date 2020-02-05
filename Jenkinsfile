pipeline {
  agent {
    docker {
      image 'node:8-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('phase1') {
      steps {
        sh 'npm install'
      }
    }

    stage('phase2') {
      steps {
        sh 'npm test'
      }
    }

  }
}