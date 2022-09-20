pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script  {
                    if (currentBuild.getBuildCauses('com.cloudbees.jenkins.GitHubPushCause') && env.BRANCH_NAME == 'main') {
                        echo "tasd"
                    } else if (currentBuild.getBuildCauses('com.cloudbees.jenkins.GitHubPushCause') && env.BRANCH_NAME != 'main') {
                        echo "!"
                    } else {
                        echo "t"
                    }
                }
            }
        }
    }
}
