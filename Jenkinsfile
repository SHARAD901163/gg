pipeline {
  agent any
  stages {
    stage('data') {
      parallel {
        stage('data') {
          steps {
            bat(script: 'date', returnStatus: true)
          }
        }

        stage('work') {
          steps {
            bat(script: 'time', returnStatus: true, returnStdout: true)
          }
        }

      }
    }

  }
}