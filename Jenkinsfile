node {
         def commitHash = checkout(scm).GIT_COMMIT
        def branch = checkout(scm).GIT_BRANCH
  sh "echo prout : ${commitHash}  ${branch}"
      shortCommit = sh(returnStdout: true, script: "git rev-parse HEAD")
     sh "echo yolo :  ${shortCommit}"
      gitbranch = sh(returnStdout: true, "git branch -f ${shortCommit}")
      sh "echo yolo :  ${gitbranch}"
}
