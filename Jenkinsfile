pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1.1') {
          steps {
            bat(script: 'echo 1.1', returnStdout: true, returnStatus: true)
          }
        }
        stage('stage1.2') {
          steps {
            bat 'echo 1.2'
          }
        }
      }
    }
  }
}