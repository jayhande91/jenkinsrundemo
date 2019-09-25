pipeline {
    agent any 
    stages {
        stage('Clone Repo') { 
            steps {
          sh "export AWS_DEFAULT_REGION=us-east-1"
          
sh "aws cloudformation create-stack --stack-name myteststack --template-body file://ec2-stack.yml --region 'us-east-1'"
          
          }
        }
        stage('Test') { 
            steps {
                sh "ls"
            }
        }
        stage('Deploy') { 
            steps {
               sh "ls"
            }
        }
    }
}
