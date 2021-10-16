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
        def listOfHosts = $HOSTS
        def hostsArray=[]
        stage('string to array') {
            steps {

                listOfHosts.split().each {
                    hostsArray << it
                }
                print hostsArray
//                sh ''' for i in $HOSTS

            }
        }
    }
}
