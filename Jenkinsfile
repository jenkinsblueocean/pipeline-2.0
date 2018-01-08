pipeline {
  agent any
  stages {
    stage('Stage 1') {
      parallel {
        stage('Stage 1') {
          steps {
            echo 'Executing without errors'
          }
        }
        stage('Stage 1 parallel') {
          steps {
            echo 'no-errors'
          }
        }
        stage('Stage 1 parallel-bis') {
          steps {
            echo 'Executing stage 1 parallel-bis no errors'
          }
        }
      }
    }
    stage('Stage 2') {
      steps {
        echo 'Executing Stage 2'
      }
    }
    stage('Stage 3') {
      steps {
        catchError() {
          error 'error'
        }
        
      }
    }
  }
}