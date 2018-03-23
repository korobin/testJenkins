pipeline {
    agent any


    stages {
        stage('Build') {
            steps {
                rev = sh(returnStdout: true, script: "git rev-parse HEAD")
                branch = sh(returnStdout: true, script: "git branch --contains ${rev}")
                sh 'echo ${rev} ${branch}'
                sh 'printenv'
                
            }
        }
    }
}

