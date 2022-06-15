pipeline {
    agent any
    stages {
      stage ('wololo') {
        steps {
            sh "echo '${JOB_NAME}' | cut -d'/' -f 2"
            sh "sh wololo.sh"
        }   
      }
    }
}
