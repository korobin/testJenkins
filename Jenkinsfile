pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
    post { 
        failure { 
            tuleapPulisher credentialsId: '', repositoryId: '125', result: 'FAIL', selectedConnection: 'test'
        }
             success{
                 tuleapPulisher credentialsId: '', repositoryId: '125', result: 'SUCCESS', selectedConnection: 'test'
             }
    }
}
