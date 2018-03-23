pipeline {
    agent any


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

