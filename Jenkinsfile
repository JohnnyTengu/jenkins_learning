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
                sh '''
                arr=($HOSTS)
                for i in arr
                do
                  echo "$i"
                done


                '''

            }
        }
    }
}
