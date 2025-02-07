pipeline {
    agent any
    stages {
        stage('Deploy to EKS') {
            steps {
                script {
                    sh 'kubectl get pods --namespace default'
                }
            }
        }
    }
}