pipeline {
    agent any
    stages{
        stage('Stage One'){
            steps{
                sh 'echo "This is to show that step one works" > file1'
            }
        }
        stage('Stage Two'){
            steps{
                sh 'echo "This is to show that step two works" > file2'
            }
        }
        stage('Stage Three'){
            steps{
                sh 'echo "This is to show that step three works" > file3'
            }
        }
    }
}