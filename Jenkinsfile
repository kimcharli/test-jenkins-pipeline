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
        input 'proceed to 201?'
        sh 'echo continuing stage 201'
        sh 'echo and continue again'
        sh 'echo check again to see McAfee'
      }
    }
  }
}