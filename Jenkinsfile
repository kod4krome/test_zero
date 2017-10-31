pipeline {
  agent any
  stages {
    stage('Wait A') {
      steps {
        sleep 30
      }
    }
    stage('Wait B') {
      steps {
        sleep 30
      }
    }
    stage('Message') {
      steps {
        echo 'Done!'
      }
    }
  }
}