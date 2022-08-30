pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo $repo
                echo "--------------- token !"
                echo "${currentBuild.buildCauses}"
                script  {
                    if (currentBuild.getBuildCauses('com.cloudbees.jenkins.GitHubPushCause') && env.BRANCH_NAME == 'main') {
                        echo "this is from webhook and main, so this will be deployed"
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
