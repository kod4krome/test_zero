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
    stage('Parallel') {
      parallel {
        stage('Wait 30') {
          steps {
            sleep 30
          }
        }
        stage('parA') {
          steps {
            sh '''date
'''
          }
        }
        stage('parB') {
          steps {
            fileExists 'one.txt'
          }
        }
      }
    }
    stage('End Message') {
      steps {
        sleep 30
      }
    }
  }
}