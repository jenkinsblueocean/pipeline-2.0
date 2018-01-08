pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        error 'errore-a-mano'
      }
    }
    stage('Stage 2') {
      steps {
        echo 'Executing Stage 2'
        error 'errore-a-mano'
      }
    }
  }
}