pipeline {
  agent any
  stages {
    stage('Ls -al') {
      steps {
        sshagent(['jenkins-ssh-key']) {
          ssh administrateur@100.64.80.33 "ls -al"
        }
      }
    }
  }
}
