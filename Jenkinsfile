pipeline {
  agent any
  stages {
    stage('test1') {
      parallel {
        stage('test1') {
          steps {
            bat(script: 'echo testtoto', returnStdout: true, returnStatus: true)
          }
        }
        stage('stage2') {
          steps {
            bat 'echo toto'
          }
        }
      }
    }
  }
}