pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1.1') {
          steps {
            bat 'echo 1.1'
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