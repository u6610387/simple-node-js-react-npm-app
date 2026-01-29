pipeline {
  agent any

  tools {
    nodejs 'Node 18'
  }

  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }

    stage('Test') {
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }
  }
}
