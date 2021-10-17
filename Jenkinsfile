pipeline {
  agent any
  stages {
    stage('clone repository') {
      steps {
        sh 'git clone git@github.com:JohnnyTengu/run_ping.git'
        sh 'ls -al'
      }
    }
  }
}