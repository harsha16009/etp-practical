pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'docker build -t int77 .'
            }
        }
        stage('Deploy'){
            steps{
                sh 'kubectl apply -f deployment.yaml'
            }
        }
    }
}
