pipeline {
    agent any
    stages {
stage('Checkout') {
 // Get CalibrationResults from GitHub
 checkout([
            $class: 'GitSCM',
            branches: [[name: 'refs/heads/master']],
            doGenerateSubmoduleConfigurations: false,
            extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'CalibrationResults']],
            submoduleCfg: [],
            userRemoteConfigs: [[credentialsId: 'f52a146e-fa29-424c-9d5a-ddae64f7343e', url: 'git@github.com:JohnnyTengu/run_ping.git']]
        ])
 // Get Combination from GitHub
}
        stage('ping') {
            steps {
                sh 'ls -al'
            }
        }
    }
}