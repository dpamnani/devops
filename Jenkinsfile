pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''echo "fenris" | sudo -S ./mvnw package
'''
        stash 'Target'
      }
    }

  }
}