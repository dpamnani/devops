pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh 'sudo ./mvnw package'
        stash 'Target'
      }
    }

  }
}