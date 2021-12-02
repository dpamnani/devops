pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo -S \\
fenris 
./mvnw package'''
        stash 'Target'
      }
    }

  }
}