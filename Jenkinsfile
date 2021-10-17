import groovy.json.JsonOutput
import jenkins.model.*

node {
    stage('ping_all_hosts') {
        def full_string = String.valueOf(HOSTS)
        def arr = full_string.split("\n")
        for (i in arr) {
          println i
          build job: 'PING', parameters: [
              string(name: 'WHAT_PING', value: String.valueOf( i ) )
              ]
        }
    }
    stage('run_ping_credentials') {
        withCredentials([string(credentialsId: 'DOMAIN', variable: 'secrets')]) {
        build job: 'PING', parameters: [string(name: 'WHAT_PING', value: String.valueOf(secrets))]
        }
    }
}