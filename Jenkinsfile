node {

      git credentialsId: '1c7ab69b-9e00-40c4-85ca-88472f49fdab', url: 'https://github.com/korobin/testJenkins.git'
         def commitHash = checkout(scm).GIT_COMMIT
        def branch = checkout(scm).GIT_BRANCH
  sh "echo prout : ${commitHash}  ${branch}"
      shortCommit = sh(returnStdout: true, script: "git rev-parse HEAD")
     sh "echo yolo :  ${shortCommit}"
      gitbranch = sh(returnStdout: true, "git branch --contains ${shortCommit}")
      sh "echo yolo :  ${gitbranch}"
}
