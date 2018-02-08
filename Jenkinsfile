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
        sh './jenkins/scripts/test.sh'
      }
    }
  }
}
