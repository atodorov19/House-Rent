pipeline{
    agent any

    stages{
        stage("Restore the project"){
            step{
                bat "dotnet restore"
            {
        }
        stage("Build the project"){
                step{
                bat "dotnet build --no-restore"
                }
        }
        stage("Run unit tests"){
                step{
                bat "dotnet test --no-build --verbosity normal"
                }
        }
    }
}
