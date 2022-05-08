pipeline {
  agent any
  stages {
    stage('date_data') {
      parallel {
        stage('date_data') {
          steps {
            bat(script: 'date', returnStatus: true, returnStdout: true)
          }
        }

        stage('time_data') {
          steps {
            bat(script: 'time', returnStatus: true, returnStdout: true)
          }
        }

      }
    }

    stage('cd_data') {
      steps {
        bat(script: 'cd', returnStatus: true, returnStdout: true)
      }
    }

  }
}