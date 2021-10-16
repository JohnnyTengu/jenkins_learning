pipeline {
    agent any
    stages {
        stage('print hosts list') {
            steps {
//                params.HOSTS
                sh 'echo "Print hosts list"'
                sh 'echo $HOSTS'
            }
        }
        stage('Ping host list') {
            steps {
                sh 'echo "step 2"'

            }
        }
    }
}
