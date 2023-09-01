pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                echo "building....."
            }
            post{
                always{
                    mail to : "minunsunil@gmail.com",
                    subject : "build status email",
                    body : "build was successfull"
                }
            }
        }
        stage("Test"){
            steps{
                echo "Testing...."
            }
        }
        stage("Deploy"){
            steps{
                echo "Deploying...."
            }
        }
        stage("Complete"){
            steps{
                echo "completed...."
            }
        }
    }    
}
