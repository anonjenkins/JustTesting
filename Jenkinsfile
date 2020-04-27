pipeline {
  agent {
    node {
      label 'BenVMNode'
    }

  }
  stages {
    stage('Run Git Pull') {
      steps {
        sh '''git pull
pwd'''
      }
    }

    stage('Run build') {
      steps {
        sh 'sudo build/run.sh make'
      }
    }

  }
}