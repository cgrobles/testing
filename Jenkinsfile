pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World over 9000'
                echo "${currentBuild.buildCauses}"
                script  {
                    if (currentBuild.getBuildCauses('com.cloudbees.jenkins.GitHubPushCause') {
                        echo "LETSGOOOO"
                    } else {
                        echo "yekale"
                    }
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
