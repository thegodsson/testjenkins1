pipeline {

  agent any

  stages {

    stage('Checkout Source') {
      steps {
        git url:'https://github.com/thegodsson/testjenkins1.git', branch:'main'
      }
    }

    stage('Deploy App') {
      steps {
        script {
          kubernetesDeploy(configs: "stack_web.yaml", kubeconfigId: "mykubeconfig")
        }
      }
    }

  }

}
