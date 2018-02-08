pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "now install npm..."'
      }
    }
    stage('Test') {
      steps {
        echo 'Now begin testing'
        sh './jenkins/scripts/test.sh'
      }
    }
  }
}