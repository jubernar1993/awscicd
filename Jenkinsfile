pipeline{
agent any
    stages{
        stage('Source Checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/jubernar1993/awscicd.git'
            }
        }
        stage('Stage #2'){
            steps{
                sh 'ls -la'
            }
        }
        stage('Stage #3'){
            steps{
                sh 'free -m'
            }
        }
    } 
}