pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo -S ferris 
./mvnw package'''
        stash 'Target'
      }
    }

  }
}