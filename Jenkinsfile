node {

      git credentialsId: 'puteuh', url: 'https://github.com/korobin/testJenkins.git'
       sh "echo ${env.BRANCH_NAME}"
         def commitHash = checkout(scm).GIT_COMMIT
        def branch = checkout(scm).GIT_BRANCH
  sh "echo prout : ${commitHash}  ${branch}"

}
