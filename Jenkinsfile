pipeline {
  agent {
    kubernetes {
      
    }
  }
  stages {
    stage('Build') {
      steps {  // TEST 1
        echo "Bonjour"   
      }
    }
    stage('TEST2') {
      steps {
        container('docker') {  
          sh "docker ps"
        }
      }
    }
  }
}
