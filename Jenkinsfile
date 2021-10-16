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
                #!/bin/bash
                myvar="string1 string2 string3 8.8.8.8 google.com test.test 123.321"
                myarray=$myvar
                echo "My array: ${myarray[@]}"
                '''

            }
        }
    }
}
