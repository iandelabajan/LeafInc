pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        bat 'start cmd.exe ssh ian@127.0.0.1'
      }
    }
	
	stage('Remote SSH') {
      steps {
        sshagent(credentials : ['ansibleId']) {
		sh 'pwd'
      }
    }
	
  }
}
