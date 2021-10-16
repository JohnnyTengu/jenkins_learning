pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                // 
            }
        }
        stage('Test') { 
            steps {
                // 
            }
        }
        stage('Deploy') { 
            steps {
                // 
            }
        }
    }
}
pipeline { 
    agent any 
    }
    stages {
        stage('Wait') { 
            steps { 
                sh 'echo "wait"' 
            }
        }
        stage('Test'){
            steps {
                sh 'ping $WHAT_PING -c 4'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploy"'
            }
        }
    }
}
