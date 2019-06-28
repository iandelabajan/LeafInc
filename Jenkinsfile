pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'hello'
      }
    }
    stage('Remote SSH') {
    steps{
        sshagent(credentials : ['ansibleId']) {
            sh 'pwd'
        }
    }
  }
    
  }
}
