pipeline {
  agent any

  environment {
        AWS_ACCESS_KEY_ID = credentials('access_key')
        AWS_SECRET_ACCESS_KEY = credentials('secret_key')
        SERVER_SSH_KEY_FILE = credentials('ssh_key')
    }
  
  stages {
    stage("echo") {
      steps {
        echo 'Cow'
      }
    }

    stage("ssh") {
      steps {
        echo 'ssh'
        
      }
    }
  }
}
