pipeline {
    agent any
    stages {
        stage('print hosts list') {
            steps {
                params.HOSTS
//                sh '''#!/bin/bash
//                        ./ping_addr.sh
//                '''
            }
        }
    }
}
