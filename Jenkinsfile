pipeline {
  agent any
  stages {
    stage('clone repository') {
      steps {
        git branch: 'main', credentialsId: 'f52a146e-fa29-424c-9d5a-ddae64f7343e', url: 'git@github.com:JohnnyTengu/run_ping.git'
        sh 'ls -al'
        sh "ls -lart ./*"
        // List all branches in your repo.
        //sh "git branch -a"
        // Checkout to a specific branch in your repo.
        //sh "git checkout master"
      }
    }
    stage('run_ping') {
      steps {
        sh 'echo $WHAT_PING'
        sh './ping.sh'
      }
    }
  }
}