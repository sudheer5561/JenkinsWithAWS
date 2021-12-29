pipeline{
    agent{
        label "master"
    }
    stages{
        stage("Verify awscli installation"){
            steps{
                sh 'aws --verison'
            }
          
        }
    }

}
