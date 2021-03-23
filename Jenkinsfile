pipeline{
    agent any

    stages{

        stage("kubernates"){
            steps{
                bat "kubectl apply -f api-deployment.yml"
                 bat "kubectl apply -f ui-deployment.yml"
                 bat "kubectl apply -f database-deployment.yml"
                 bat "kubectl apply -f autoscaling.yml"
            }
        }
    }
}
