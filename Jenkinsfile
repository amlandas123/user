@Library("jenkins-shared-library") _
pipeline{
    agent{
        label "node"
    }
    stages{
        stage("Lintchecks"){
            steps{
                 script {
                    nodejs.lintchecks()
                }
                
            }
            
        }
        stage("Static code analysic"){
            steps{
                sh "echo Static code analysis "
            }
        }
    }
    
}