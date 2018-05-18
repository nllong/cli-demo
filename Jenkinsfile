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
            sh 'echo "what is next  not this"'
          }
        }
      }
    }
  }
}
