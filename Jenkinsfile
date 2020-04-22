pipeline {
  agent {
    node {
      label 'BenVMNode'
    }

  }
  stages {
    stage('Run Git Pull') {
      steps {
        sh 'git pull'
      }
    }

  }
}