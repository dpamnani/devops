pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo -S ./mvnw package
echo "fenris"
'''
        stash 'Target'
      }
    }

  }
}