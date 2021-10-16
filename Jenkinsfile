pipeline {
    agent any
    stages {
        stage('ping') {
            steps {
                sh '''#!/bin/bash
                        ./ping_addr.sh
                '''
            }
        }
    }
}