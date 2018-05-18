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
    stage('lkj') {
      steps {
        input(message: 'are we done?', id: '5', ok: 'yes')
      }
    }
    stage('artifacts') {
      steps {
        archiveArtifacts '*'
      }
    }
  }
}