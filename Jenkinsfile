pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script  {
                    if (currentBuild.getBuildCauses('com.cloudbees.jenkins.GitHubPushCause') && env.BRANCH_NAME == 'main') {
                        echo "th"
                    } else if (currentBuild.getBuildCauses('com.cloudbees.jenkins.GitHubPushCause') && env.BRANCH_NAME != 'main') {
                        echo "skipping this build!"
                    } else {
                        echo "this is a manual execution"
                    }
                }
            }
        }
    }
}
