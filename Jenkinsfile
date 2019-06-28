pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'hello'
      }
    }
    stage('error') {
      steps {
        sh '''ssh ian@127.0.0.1
pwd
ls'''
      }
    }
  }
}