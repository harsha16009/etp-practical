pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'docker build -t int77 .'
            }
        }
        stage('push'){
            steps{
                sh 'docker push int77'
            }
        }
        stage('Deploy'){
            steps{
                sh 'kubectl apply -f deployment.yaml'
            }
        }
    }
}