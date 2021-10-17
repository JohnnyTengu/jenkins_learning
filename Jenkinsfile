pipeline {
  agent any
  stages {
    stage('run_ping_job') {
      steps {
        build job: 'PING', parameters: [string(name: 'WHAT_PING', value: '$HOSTS')]
        //sh 'echo $WHAT_PING'
        //sh './ping.sh'
      }
    }
    //stage('run_ping_credentials') {
      //steps {
        //sh 'echo $WHAT_PING'
        //sh './ping.sh'
      //}
    //}
  }
}