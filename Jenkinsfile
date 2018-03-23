pipeline {
    agent any

    environment {
        TULEAP_GIT_COMMIT = $(git rev-parse HEAD)
        TULEAP_GIT_BRANCH  = "${GIT_BRANCH#*/}"
    }

    stages {
        stage('Build') {
            steps {
                rev=$(git rev-parse HEAD)
                branch="${GIT_BRANCH#*/}"
                sh 'echo ${rev} ${branch}'
                sh 'printenv'
                
            }
        }
    }
}

