pipeline{
    agent any
    
    environment{
        BRANCH_NAME= 'main'
        GIT_URL= 'https://github.com/jubernar1993/awscicd.git'
        IMAGE_TAG= 'awscicd'
        IMAGE_VERSION= "${BUILD_NUMBER}"
    }
    stages{
        stage('Code Checkout'){
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }

        stage('Docker Build'){
            steps{
                sh 'docker build -t "${IMAGE_TAG}":"${IMAGE_VERSION}" .'
                sh 'docker images'
            }
        }

    }
}