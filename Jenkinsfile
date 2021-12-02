pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh 'mvn package'
        stash 'Target'
      }
    }

  }
}