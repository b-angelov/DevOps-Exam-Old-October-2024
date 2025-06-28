pipeline{
    agent any

    stages{

        stage("CHeckout SCM"){
            steps{
                checkout scm
            }
        }

        stage("Build App"){
            steps{
                bat 'dotnet build'
            }
        }

        stage("Test App"){
            steps{
                bat 'dotnet test --no-build --verbosity normal'
            }
        }
    }
}