pipeline {
  agent any
  stages {
    stage('stage 101') {
      parallel {
        stage('stage 101') {
          steps {
            echo 'message from stage 101'
            input 'are you ok to proceed?'
          }
        }
        stage('stage 102') {
          steps {
            sh 'echo echo from stage 102'
          }
        }
      }
    }
    stage('stage 201') {
      steps {
        input(message: 'proceed to 201?', id: 'stage_201')
      }
    }
  }
}