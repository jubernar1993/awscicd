pipeline{
agent any

enviroment{
    BRANCH_NAME = 'main'
    GIT_URL = 'https://github.com/jubernar1993/awscicd.git'
}
    stages{
        stage('Source Checkout'){
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
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