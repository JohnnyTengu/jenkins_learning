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
        stage('string to array') {
            steps {
            sh '''/usr/bin/python3
            hosts=$HOSTS
            print(hosts)
            '''
            }
        }
    }
}
