pipeline {
    agent any
    environment {
        KUBECONFIG = "/var/lib/jenkins/.kube/config"
    }
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