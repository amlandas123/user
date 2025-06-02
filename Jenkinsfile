pipeline{
    agent {
        label 'ws'
    }
    stages{
        stage('lint checks'){
            steps{
                sh "echo ***********Starting Style Checks****************"
                sh "/home/ec2-user/node_modules/jslint/bin/jslint.js server.js || true"
            }
        }    
        stage('Static Code Analysis'){
            steps{
                sh "echo ******** Starting Static Code Analysis *******"
                sh "echo welcome all to sonarcube"
            }
        }
    }
    
}
