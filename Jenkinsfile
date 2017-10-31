pipeline {
  agent any
  stages {
    stage('Start Message') {
      steps {
        echo 'Begin!'
      }
    }
    stage('Status') {
      steps {
        sh '''git status
'''
      }
    }
    stage('Wait 30') {
      steps {
        sleep 30
      }
    }
    stage('End Message') {
      steps {
        sleep 30
      }
    }
  }
}