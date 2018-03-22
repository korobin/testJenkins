node {

        git credentialsId: '47814913-e78c-438d-94a5-17dda6be8235', url: 'https://github.com/korobin/testJenkins.git'
        sh "echo ${env.BRANCH_NAME}"
         
         def commitHash = checkout(scm).GIT_COMMIT
         sh "echo prout : ${commitHash}"
}
