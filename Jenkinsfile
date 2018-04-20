node {
         def commitHash = checkout(scm).GIT_COMMIT
        def branch = checkout(scm).GIT_BRANCH
          checkout scm
  sh "echo prout : ${commitHash}  ${branch}"
      shortCommit = sh(returnStdout: true, script: "git rev-parse HEAD")
     sh "echo yolo :  ${shortCommit}"
         tuleapPublisher credentialsId: '', repositoryId: '1547', result: 'ABORTED', selectedConnection: 'test'
}
