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
        bat 'ssh ian@127.0.0.1'
        bat 'ls'
      }
    }
  }
}