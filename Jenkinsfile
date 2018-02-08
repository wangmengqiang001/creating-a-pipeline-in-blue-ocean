pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "now install npm..."'
          }
        }
        stage('buid module-2') {
          steps {
            sh 'echo "building 2nd Module"'
          }
        }
      }
    }
    stage('Test') {
      environment {
        CI = 'TRUE'
      }
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }
  }
}