pipeline {
  agent {
    docker {
      image 'node:10'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }
    stage('') {
      steps {
        sh 'npm run build'
      }
    }
  }
}