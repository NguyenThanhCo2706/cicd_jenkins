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
        chmod 400 $SERVER_SSH_KEY_FILE
        ssh -o StrictHostKeyChecking=no -i $SERVER_SSH_KEY_FILE  ubuntu@ec2-54-252-234-125.ap-southeast-2.compute.amazonaws.com "
"
      }
    }
  }
}
