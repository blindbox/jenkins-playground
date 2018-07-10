pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'node:10-alpine'
    }

  }
  stages {
    stage('Install') {
      steps {
        sh 'yarn'
      }
    }
    stage('build') {
      steps {
        sh 'npm run build'
      }
    }
  }
}