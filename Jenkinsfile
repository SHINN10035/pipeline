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
        sh 'composer install'
      }
    }
    stage('Artifacts') {
      steps {
        sh 'tar -czf dist.tar.gz ./dist'
        stash 'dist.tar.gz'
      }
    }
}
}
