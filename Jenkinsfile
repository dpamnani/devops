pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo -s ./mvnw package
echo "fenris"
'''
        stash 'Target'
      }
    }

  }
}