pipeline:
agent any
    stages{
        stage('Stage #1'){
            steps{
                sh 'echo "Well i Guess this works! > /home/stage1"'
            }
        }
        stage('Stage #2'){
            steps{
                sh 'cat /home/stage1'
            }
        }
        stage('Stage #3'){
            steps{
                sh 'rm -rf /home/stage1'
            }
        }
    } 