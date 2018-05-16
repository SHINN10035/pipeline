pipeline {
  agent any
  stages {
    stage('Information') {
      steps {
        sh 'node -v'
        sh 'npm -v'
      }
    }
    stage('Dependencies') {
      steps {
        sh 'composer update'
      }
    }
    stage('Artifacts') {
      steps {
        sh 'touch 1.txt
      }
    }
  }
}
