pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'hello'
      }
    }
    stage('ansible') {
      steps {
        ansiblePlaybook(playbook: 'ansible', credentialsId: 'ian')
      }
    }
  }
}