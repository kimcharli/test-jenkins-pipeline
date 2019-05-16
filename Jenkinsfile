pipeline {
  agent any
  stages {
    stage('stage 101') {
      parallel {
        stage('stage 101') {
          steps {
            echo 'message from stage 101'
            input(message: 'are you ok to proceed?', id: 'stage_101')
          }
        }
        stage('stage 102') {
          steps {
            sh 'echo echo from stage 102'
          }
        }
      }
    }
  }
}