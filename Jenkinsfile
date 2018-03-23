node{
                shortCommit = sh(returnStdout: true, script: "git log -n 1 --pretty=format:'%h'").trim()
                def rev = sh(returnStdout: true, script: "git rev-parse HEAD")
                def  branch = sh(returnStdout: true, script: "git branch --contains ${rev}")
                sh 'echo ${rev} ${branch}'
                sh 'printenv'
                
        }
