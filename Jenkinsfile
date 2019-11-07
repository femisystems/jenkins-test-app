pipeline {
  agent {
    docker {
      image: 'node:10'
    }
  }
  stages {
    stage('install') {
      steps {
        sh 'npm install'
      }
    }
    stage('build') {
      steps {
        sh 'echo "Building application"'
        sh 'npm run build'
        sh 'echo "starting application"'
        sh 'npm start'
      }
    }
  }
}
