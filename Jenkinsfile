pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1.1') {
          steps {
            sh "echo 1.1 test again..."
          }
        }
        stage('stage1.2') {
          steps {
            sh "echo 1.2"
          }
        }
      }
    }
    stage('stage2') {
      steps {
        sh "sleep 10"
      }
    }
    stage('stage3') {
      steps {
        sh "echo stage3"
      }
    }
  }
}
