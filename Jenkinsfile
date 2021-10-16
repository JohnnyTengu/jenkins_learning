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
}
        stage('string to array') {
            steps {
                script {
//                    def listCatalog = sh script: "ls src/examplecatalog", returnStdout: true
                    def listCatalog = $HOSTS
                    def arrayExample=[]
                    listCatalog.split().each {
                    arrayExample << it
            }
            echo "${arrayExample}"
                }
                sh 'array=$HOSTS'
                sh 'echo "{$array[@]}"'

            }
        }
    }

