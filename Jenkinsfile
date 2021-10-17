pipeline {
  agent any
  stages {
    stage('run_ping_job') {
      steps {
        sh 'echo $HOSTS'
        build job: 'PING', parameters: [string(name: 'WHAT_PING', value: String.valueOf(HOSTS))]
        //sh 'echo $WHAT_PING'
        //sh './ping.sh'
      }
    }
    stage('run_ping_credentials') {
      steps {
        build job: 'PING', parameters: [string(name: 'WHAT_PING', value: String.valueOf(CREDSECRET))]
      }
    }
  }
}