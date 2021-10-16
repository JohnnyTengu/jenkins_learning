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
                def listOfHosts = $HOSTS
                def hostsArray=[]
                listOfHosts.split().each {
                    hostsArray << it
                }
                print hostsArray
//                sh ''' for i in $HOSTS

            }
        }
    }
}
