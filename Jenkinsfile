pipeline{
    agent any
    stages{
        stage("Restore dependencies"){
             steps{
                echo "dotnet restore"
            }
        }

        stage("Build"){
             steps{
                echo "dotnet build"
            }
        }

        stage("Run tests"){
             steps{
                echo "dotnet test"
            }
        }
    }
    post{
        success{
            echo "Workflow executed successfully"
        }
        failure{
            echo "Workflow execution failed"
        }
    }
}