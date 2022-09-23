pipeline {
    agent any

    stages {
        stage('Read properties') {
            steps {
                script  {
                    props = readProperties file: './sonar.properties'
                }
                echo "doing a test ${props['sonar.property']}"
                echo "doing a test ${props['sonar.test']}"
                sh "curl -u ${props['sonar.property']} -X GET http://localhost:8080"
            }
        }
    }
}
