import groovy.json.JsonOutput
import jenkins.model.*

node {
    stage('test') {
        def full_string = String.valueOf(HOSTS)
        def arr = full_string.split(" ")
        for (i in arr) {
          build job: 'PING', parameters: [
              string(name: 'WHAT_PING', value: String.valueOf( i ) )
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