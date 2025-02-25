pipeline{
agent any

environment{
    BRANCH_NAME = 'main'
    GIT_URL = 'https://github.com/jubernar1993/awscicd.git'
}
    stages{
        stage('Source Checkout'){
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }
        stage('Docker Build'){
            steps{
                sh 'docker build -t awscicd .'
                sh 'docker images'
            }
        }
        stage('Stage #3'){
            steps{
                sh 'free -m'
            }
        }
    } 
}