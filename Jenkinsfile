pipeline {
   agent any

    environment {
        SERVER_USERNAME = credentials('SERVER_USERNAME')
        SERVER_URL = credentials('SERVER_URL')

        SERVER_SSH_KEY_FILE = credentials('SSH_KEY_FILE')
    }

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
               sh 'chmod +x ./deploy.sh && ./deploy.sh'
          }
      }
   }
}
