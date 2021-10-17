import groovy.json.JsonOutput
import jenkins.model.*

node {
    stage('test') {
        def full_string = String.valueOf(HOSTS)
        def arr = full_string.split(" ")
        for (i in arr) {
          println "now got ${i}"
          build job: 'PING', parameters: [
              string(name: 'WHAT_PING', value: String.valueOf( i ) )
              ]
}


    }
}