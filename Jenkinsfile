pipeline {
    agent any

    environment {
        TULEAP_GIT_COMMIT = $(git rev-parse HEAD)
        TULEAP_GIT_BRANCH  = "${GIT_BRANCH#*/}"
    }

    stages {
        stage('Build') {
            steps {
                TULEAP_GIT_COMMIT = checkout(scm).GIT_COMMIT
                TULEAP_GIT_BRANCH  = checkout(scm).GIT_BRANCH
                sh 'printenv'
                
            }
        }
    }
}

