node{ 
  git credentialsId: '1c7ab69b-9e00-40c4-85ca-88472f49fdab', url: 'https://github.com/korobin/testJenkins.git'
        sh "echo ${env.BRANCH_NAME}"
         def commitHash = checkout(scm).GIT_COMMIT
         def branch = checkout(scm).GIT_BRANCH
         sh "echo prout : ${commitHash}  ${branch}"
                
        }
