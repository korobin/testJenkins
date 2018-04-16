pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                //script {omg}
            }
        }
    }
    post { 
        failure { 
            tuleapPublisher credentialsId: '', repositoryId: '125', result: 'FAIL', selectedConnection: 'test'
        }
             success{
                 tuleapPublisher credentialsId: '', repositoryId: '125', result: 'SUCCESS', selectedConnection: 'test'
             }
    }
}
