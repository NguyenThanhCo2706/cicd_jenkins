pipeline {
  agent any
  tools {
    nodejs '21.7.1'
  }
  stages {
    stage("checkout") {
      steps {
        checkout scm
      }
    }

    stage("install") {
      steps {
        sh 'npm install'
      }
    }

    stage('Install pm2'){
      steps {
          sh 'npm install pm2 -g'
      }
    }

    stage("start") {
      steps {
        sh 'pm2 start server.js'
      }
    }
  }
}
