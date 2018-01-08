pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        echo 'Executing without errors'
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