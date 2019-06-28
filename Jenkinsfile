pipeline {
  agent {
    node {
      label 'test'
    }

  }
  stages {
    stage('test') {
      steps {
        bat 'start cmd.exe ssh ian@127.0.0.1'
      }
    }
  }
}