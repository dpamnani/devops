pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo -S
echo "fenris" 
./mvnw package'''
        stash 'Target'
      }
    }

  }
}