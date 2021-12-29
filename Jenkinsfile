pipeline{
    agent{
        label "master"
    }
    stages{
        stage("Verify awscli installation"){
            steps{
                script{
                      sh 'aws --version'
                }
              
            }
          
        }
    }

}
