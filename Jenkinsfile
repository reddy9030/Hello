pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo "bild with Maven"
                }
        }
        stage('upload to nexus'){
            steps{
                echo "upload to nexus"
                }
        }
        stage('Deploy to Dev'){
            when {
                branch 'develop'
            }
            steps{
                echo "deploy to dev"
                }
        }
        stage('Deploy to Test'){
            when {
                branch 'test'
            }
            steps{
                echo "deploy to test"
                }
        }
        stage('Deploy to Prod'){
            when {
                branch 'master'
            }
            steps{
                echo "deploy to prod"
                }
        }
    }
}