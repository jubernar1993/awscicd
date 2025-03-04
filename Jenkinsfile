pipeline{
    agent any
    stages{
        stage('Code Checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/jubernar1993/awscicd.git'
            }
        }

        stage('Test'){
            steps{
                sh 'echo "This is a test stage"'
            }
        }

    }
}