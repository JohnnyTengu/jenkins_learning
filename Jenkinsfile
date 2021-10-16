pipeline {
  agent any
  stages {
    stage('print hosts list') {
        steps {
          script {
            def browsers = ['chrome', 'firefox']
            for (int i = 0; i < browsers.size(); ++i) {
            echo "Testing the ${browsers[i]} browser"
          }
        }
    }
  }
}
