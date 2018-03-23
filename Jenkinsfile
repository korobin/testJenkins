pipeline {
    agent any

    environment {
        TULEAP_GIT_COMMIT = $(git rev-parse HEAD)
        TULEAP_GIT_BRANCH  = "${GIT_BRANCH#*/}"
    }

    stages {
        stage('Build') {
            steps {
                sh 'printenv'
                
            }
        }
    }
}

