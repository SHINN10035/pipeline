pipeline {
  agent any
  stages {
    stage('Information') {
      steps {
        sh 'node -v'
        sh 'npm -v'
        sh 'composer -v'
      }
    }
    stage('Dependencies') {
      steps {
        sh 'composer install'
      }
    }
    stage('Artifacts') {
      steps {
        sh 'touch 1.txt'
      }
    }
  }
}
