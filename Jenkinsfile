pipeline{
    agent any
    stages{
        stage("build"){
            steps{
                echo "building....."
            }
            post{
                success{
                    mail to : "minunsunil@gmail.com",
                    subject : "build status email",
                    body : "build was successfull"
                }
            }
        }
    }
}