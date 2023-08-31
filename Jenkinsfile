pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                echo "Building ..."
            }
            post{ //send email
                    success{
                        mail to: "hieunguyen23032001@gmail.com",
                        subject: "Build Status Email",
                        body: "Build was successfull"
                    }
                }
            }
        }
    }