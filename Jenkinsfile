pipeline {
  agent {
    kubernetes {
      
    }
  }
  stages {
    stage('Build') {
      steps {  // no container directive is needed as the maven container is the default
        sh "docker pull nginx"   
      }
    }
    stage('Build Docker Image') {
      steps {
        container('docker') {  
          sh "echo Fin"
          sh "echo FIN 2"
        }
      }
    }
  }
}
