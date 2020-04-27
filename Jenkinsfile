pipeline {
  agent {
    node {
      label 'BenVMNode'
    }

  }
  stages {
    stage('Run Git Pull') {
      steps {
        sh '''cd /home/ben/kubernetes
git pull
pwd'''
      }
    }

    stage('Run build') {
      steps {
        sh '''cd /home/ben/kubernetes
sudo build/run.sh make'''
      }
    }

  }
}