pipeline {
    agent any
    stages {
            stage('Checkout') {
      steps {
        script {
           // The below will clone your repo and will be checked out to master branch by default.
           git credentialsId: 'f52a146e-fa29-424c-9d5a-ddae64f7343e', url: 'git@github.com:JohnnyTengu/run_ping.git'
           // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
           sh "ls -lart ./*"
           // List all branches in your repo.
//           sh "git branch -a"
           // Checkout to a specific branch in your repo.
//           sh "git checkout branchname"
          }
       }
    }
        stage('ping') {
            steps {
                sh '''#!/bin/bash
                        ./run_ping/ping.sh
                '''
            }
        }
    }
}