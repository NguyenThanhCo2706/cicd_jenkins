pipeline {
   agent any
   AWS_ACCESS_KEY_ID = credentials('access_key')
        AWS_SECRET_ACCESS_KEY = credentials('secret_key')
        SERVER_SSH_KEY_FILE = credentials('ssh_key')
   stages {
       stage('Build Code') {
           steps {
               sh """
               echo "Building Artifact from Develop Branch"
               """
           }
       }
      stage('Deploy Code') {
          steps {
               sh """
               echo "Deploying Code from Develop Branch"
               """
          }
      }
   }
}
