pipeline {
  agent any
  stages {
    stage("checkout") {
      steps {
        checkout scm
      }
    }

    stage("install") {
      steps {
        sh `npm install`
      }
    }

    stage("start") {
      steps {
        sh `npm start`
      }
    }
  }
}
