pipeline {
    agent any
    stages {
        stage('download ping script') {
            steps {
                git changelog: false, credentialsId: 'jenkins', url: 'git@github.com:JohnnyTengu/run_ping.git'
                sh 'git pull'
                sh 'ls -al'
            }
        }
    }
}