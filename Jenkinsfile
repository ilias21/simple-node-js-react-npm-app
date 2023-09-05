pipeline {
  agent {
    docker {
      args '-p 3000:3000'
      image 'node:18.17.1-alpine3.18'
    }

  }
  stages {
    stage('welcome') {
      steps {
        sh 'echo "coucou"'
      }
    }

    stage('installer') {
      steps {
        sh 'npm install'
        sh 'npm run build'
      }
    }

    stage('deploy') {
      steps {
        sh 'echo "coucou"'
      }
    }

  }
}