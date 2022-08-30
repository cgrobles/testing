pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World over 9000'
                if (env.BRANCH_NAME == 'main') {
                    echo 'works!'
                }
            }
        }
    }
}
