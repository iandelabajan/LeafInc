pipeline {
  environment {
     remote = [:]
     remote.name = 'test'
  remote.host = '127.0.0.1'
  remote.user = 'ian'
  remote.password = 'devops'
  remote.allowAnyHosts = true
   }
  agent any
  stages {
    stage('test') {
      steps {
        echo 'hello'
      }
    }
    stage('Remote SSH') {
    sshCommand remote: remote, command: "ls -lrt"
  }
  }
}
