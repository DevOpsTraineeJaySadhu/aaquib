pipeline {
    agent any
    stages {
        stage("Branch Check") {
            steps {
                script {
                    def branchName = env.BRANCH_NAME
                    echo "This is the current branch: ${branchName}"

                    if (branchName == 'main') {
                        echo "This is from Master (main) branch"
                    } else if (branchName == 'dev') {
                        echo "This is from Dev branch"
                    } else if (branchName == 'stage') {
                        echo "This is from Stage branch"
                    } else {
                        echo "This is from an unknown branch: ${branchName}"
                    }
                }
            }
        }
    }
}
