pipeline {
    agent any
    stages {
        stage('Authenticate with IRSA') {
            steps {
                script {
                    sh """
                    echo "Updating kubeconfig with IRSA..."
                    aws eks update-kubeconfig --name serious-disco-sculpture --region us-east-1

                    echo "Verifying Kubernetes Connection..."
                    kubectl get nodes
                    """
                }
            }
        }
    }
}
