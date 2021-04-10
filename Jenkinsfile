pipeline{
  agent any
  stages{
    stage('Deploy'){
      steps{
        sh 'kubectl apply -f angular-pod.yaml'
        sh 'kubectl apply -f angular-svc.yaml'
        sh 'kubectl apply -f express-pod.yaml'
        sh 'kubectl apply -f express-svc.yaml'
        sh 'kubectl apply -f mongo-pod.yaml'
        sh 'kubectl apply -f mongo-svc.yaml'
      }
    }
  }
}
