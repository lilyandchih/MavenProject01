pipeline {
  agent any
  stages {
    stage('step1') {
      environment {
        a = 'aaaaaa'
      }
      parallel {
        stage('step1') {
          steps {
            echo 'step1'
          }
        }
        stage('') {
          steps {
            echo 'a'
            echo 'b'
            sh 'echo ${a}'
          }
        }
      }
    }
  }
}