pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script  {
                    if (currentBuild.getBuildCauses('com.cloudbees.jenkins.GitHubPushCause') && env.BRANCH_NAME == 'main') {
                        echo "t"
                    } else if (currentBuild.getBuildCauses('com.cloudbees.jenkins.GitHubPushCause') && env.BRANCH_NAME != 'main') {
                        echo "skipping thbuild!"
                    } else {
                        echo "this is a manual execution"
                    }
                }
            }
        }
    }
}
