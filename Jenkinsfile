pipeline {
  agent any
  stages {
    stage('Ls -al') {
      parallel {
        stage('Ls -al') {
          steps {
            sshagent(credentials: ['jenkins-ssh-key']) {
              sh 'ssh administrateur@100.64.80.33 "ls -al"'
            }

          }
        }
        stage('step 1') {
          steps {
            sh 'ls -al'
          }
        }
      }
    }
  }
}