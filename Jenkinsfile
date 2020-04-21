pipeline {
  agent {
    docker {
      image 'node:latest'
      args '-p 3001:3000'
    }

  }
  stages {
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }

    stage('Run') {
      steps {
        sh 'npm start'
      }
    }

  }
}