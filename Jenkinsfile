@Library("jenkins-shared-library") _
pipeline{
    agent{
        label "node"
    }
    stages{
        stage("Lintchecks"){
            steps{
                 script {
                    sample.info("user")
                }
                sh "whoami"
                sh "echo *** Lint check starting ***"
                sh "npm i jslint"
                sh "/home/centos/node_modules/jslint/bin/jslint.js server.js || true"
                sh "echo *** Lint check completed ***"
            }
            
        }
        stage("Static code analysic"){
            steps{
                sh "echo Static code analysis "
            }
        }
    }
    
}