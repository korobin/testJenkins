pipeline {
    agent any


    stages {
        stage('Build') {
            steps {
                def rev = sh(returnStdout: true, script: "git rev-parse HEAD")
                def  branch = sh(returnStdout: true, script: "git branch --contains ${rev}")
                sh 'echo ${rev} ${branch}'
                sh 'printenv'
                
            }
        }
    }
}

