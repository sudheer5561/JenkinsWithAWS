pipeline{

    agent{
        label "master"
    }
    stages{
        stage("Verify awscli installation"){
            steps{
                script{
                      sh '''
                      withCredentials([<object of type com.cloudbees.jenkins.plugins.awscredentials.AmazonWebServicesCredentialsBinding>]) {
                      aws --version
                      aws ec2 describe-instances
                      '''
                }
                   }
            
                }
              
            }
          
        }
    }
