pipeline {
  agent any
  stages {
    stage('stage 1') {
      parallel {
        stage('stage 1') {
          steps {
            sh 'ping -c 12 localhost'
          }
        }
        stage('stage 2') {
          steps {
            timeout(time: 10) {
              sh 'ping -c 100 localhost'
            }

          }
        }
      }
    }
  }
}