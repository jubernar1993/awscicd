pipeline{
    agent any
    environment{
        BRANCH_NAME= 'main'
    }
    stages{
        stage('Code Checkout'){
            steps{
                git branch: "${BRANCH_NAME}", url: 'https://github.com/jubernar1993/awscicd.git'
            }
        }

        stage('Test'){
            steps{
                sh 'echo "This is a test stage"'
            }
        }

    }
}