pipeline {
    agent any
    stages {
//            stage('git pull script') {
//      steps {
//        script {
//           // The below will clone your repo and will be checked out to master branch by default.
//           git credentialsId: 'f52a146e-fa29-424c-9d5a-ddae64f7343e', url: 'git@github.com:JohnnyTengu/run_ping.git'
//           // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
////           sh "ls -lart ./*"
//           // List all branches in your repo.
////           sh "git branch -a"
//           sh "git pull"
//           // Checkout to a specific branch in your repo.
////           sh "git checkout master"
//          }
//       }
//    }
        stage('ping') {
            steps {
                sh './ping_addr.sh'
            }
        }
    }
}