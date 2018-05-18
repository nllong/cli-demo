pipeline {
  agent any
  stages {
    stage('run') {
      parallel {
        stage('run') {
          steps {
            sh 'echo "hello, i love you"'
          }
        }
        stage('run parallel') {
          steps {
            error 'what the hell'
          }
        }
      }
    }
  }
}