pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World over 9000'
                echo getBuildCauses
                script  {
                    if (env.BRANCH_NAME == 'main') {
                        echo 'works!'
                    } else {
                        echo 'yeah!'
                    }
                }
            }
        }
    }
}
