pipeline {
    agent any
    stages {
        stage('download ping script') {
            steps {
                git credentialsId: 'f52a146e-fa29-424c-9d5a-ddae64f7343e', url: 'git@github.com:JohnnyTengu/run_ping.git'
                sh 'git pull'
                sh 'ls -al'
            }
        }
    }
}