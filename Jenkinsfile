pipeline {
  agent {
    dockerfile true
  }
  stages {
    stage('Prep') {
      steps {
        sh 'apk update'
        sh 'apk add git'
        sh 'yarn add jest'
      }
    }
    stage('Test') {
      steps {
        sh 'yarn run test'
      }
    }
  }
}
