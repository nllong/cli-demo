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
      parallel {
        stage('artifacts') {
          steps {
            archiveArtifacts '*'
          }
        }
        stage('asdf') {
          steps {
            timeout(time: 180, activity: true, unit: 'MINUTES') {
              echo 'What is going on'
              script {
                rake -T
              }

            }

          }
        }
      }
    }
  }
}