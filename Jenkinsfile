pipeline{

    agent{
        label "master"
    }
    stages{
        stage("Verify awscli installation"){
            steps{
                script{
                    withCredentials([<object of type com.cloudbees.jenkins.plugins.awscredentials.AmazonWebServicesCredentialsBinding>]) {
                    sh '''
                      aws --version
                      aws ec2 describe-instances
                      '''
                    }
                   }
            
                }
              
            }
          
        }
    }
