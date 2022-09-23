pipeline {
    agent any

    stages {
        stage('Read properties') {
            steps {
                script  {
                    props = readProperties file: './testing/sonar.properties'
                }
                echo "doing a test ${props['sonar.property']}"}
                echo "doing a test ${props['sonar.test']}"
            }
        }
    }
}
