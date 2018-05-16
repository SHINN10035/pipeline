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
        sh 'jar -cvf pipeline.war ./*'
        sh 'scp -r ./* root@106.14.159.47:/home/pipeline/'
      }
    }
  }
}
