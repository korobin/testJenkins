node {
         def commitHash = checkout(scm).GIT_COMMIT
         def branch = checkout(scm).GIT_BRANCH
         sh "echo prout : ${commitHash}  ${branch}"
}
