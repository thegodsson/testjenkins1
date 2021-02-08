pipeline {
  agent {
    kubernetes {
      
    }
  }
  stages {
    stage('Build') {
      steps {  // TEST 1
        sh "kubectl get all -n jenkins"   
      }
    }
    stage('TEST2') {
      steps {
        container('docker') {  
          sh "echo FIN"
        }
      }
    }
  }
}
