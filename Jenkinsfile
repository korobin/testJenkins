node {
    try{
        git credentialsId: '47814913-e78c-438d-94a5-17dda6be8235', url: 'https://github.com/korobin/testJenkins.git'
        sh "echo ${env.BRANCH_NAME}"
         def commitHash = checkout(scm).GIT_COMMIT
         def branch = checkout(scm).GIT_BRANCH
         sh "echo prout : ${commitHash}"
    }catch(e){
}finally{
    zendTuleap branchName: 'prout', connexionSelected: 'fefefef', credentialsId: 'be005304-59f0-4b75-b819-6dc9384a6e00', idRepo: '525'
         aaaSendTuleap branchName: 'bleu', connexionSelected: 'fefefef', credentialsId: 'be005304-59f0-4b75-b819-6dc9384a6e00', idRepo: '123'    }
}
