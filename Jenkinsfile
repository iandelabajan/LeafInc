pipeline {
    agent { label 'master' }
    stages {
        stage('SSH') {
            steps {
              bat 'start cmd.exe ssh unixuser@127.0.0.1 ; pwd ; ls '
            }
        }
    }
}
