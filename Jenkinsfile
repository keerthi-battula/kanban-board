pipeline{
    agent any

    stages{

        stage("kubernates"){
            steps{
                sh "kubectl apply -f api-deployment.yml"
                 sh "kubectl apply -f ui-deployment.yml"
                 sh "kubectl apply -f database-deployment.yml"
                 sh "kubectl apply -f autoscaling.yml"
            }
        }
    }
}
