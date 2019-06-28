pipeline {
  agent any
  def remote = [:]
  remote.name = 'test'
  remote.host = '127.0.0.1'
  remote.user = 'ian'
  remote.password = 'devops'
  remote.allowAnyHosts = true
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
    stage('Remote SSH') {
    sshCommand remote: remote, command: "ls -lrt"
  }
  }
}
