pipeline{
  agent any
  stages{
    stage('Deploy'){
      steps{
        sh 'kubectl apply -f angular.yaml'
        sh 'kubectl apply -f angular-svc.yaml'
        sh 'kubectl apply -f express.yaml'
        sh 'kubectl apply -f mongo.yaml'
      }
    }
  }
}
