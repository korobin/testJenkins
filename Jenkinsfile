pipeline {
    agent any

    environment {
        TULEAP_GIT_COMMIT = "" 
        TULEAP_GIT_BRANCH  = ""
    }

    stages {
        stage('Build') {
            steps {
                sh 'printenv'
                  sh "echo prout : ${env.TULEAP_GIT_COMMIT}  ${env.TULEAP_GIT_BRANCH}"
                env.TULEAP_GIT_COMMIT = checkout(scm).GIT_COMMIT
                env.TULEAP_GIT_BRANCH  = checkout(scm).GIT_BRANCH
                
            }
        }
    }
}

