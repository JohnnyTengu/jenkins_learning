import groovy.json.JsonSlurper
import jenkins.model.*

pipeline {
  agent any
  stages {
//    stage('run_ping_job') {
//      steps {
//        sh 'echo $HOSTS'
//        build job: 'PING', parameters: [string(name: 'WHAT_PING', value: String.valueOf(HOSTS))]
        //sh 'echo $WHAT_PING'
        //sh './ping.sh'
//      }
//    }
    stage('test') {
        //def myArray = string(name: 'myParam', value: String.valueOf(ARRAY))
        //print myArray
        def full_string = String.valueOf(HOSTS)
        def arr = full_string.split(" ")
        for (i in arr) {
          println "now got ${i}"
          build job: 'CalledPipeline', parameters: [
              string(name: 'myParam', value: JsonOutput.toJson( i ) )
              ]
        }
      }
    stage('run_ping_credentials') {
      steps {
        withCredentials([string(credentialsId: 'DOMAIN', variable: 'secrets')]) {
    // some block

        build job: 'PING', parameters: [string(name: 'WHAT_PING', value: String.valueOf(secrets))]
        }
      }
    }
  }
}