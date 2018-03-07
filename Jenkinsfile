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
    stage('stage2') {
      steps {
        bat 'explorer'
      }
    }
    stage('stage3') {
      steps {
        mail(subject: 'test stgae3', body: 'test', from: 'blueocean', to: 'bigjimcp660@gmail.com')
      }
    }
  }
}