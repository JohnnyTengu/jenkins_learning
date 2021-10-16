        def listOfHosts = $HOSTS
        def hostsArray=[]
        listOfHosts.split().each {
        hostsArray << it
        }
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


                print hostsArray
//                sh ''' for i in $HOSTS

            }
        }
    }
}
