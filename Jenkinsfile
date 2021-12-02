pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo ./mvnw package
echo "fenris"
'''
        stash 'Target'
      }
    }

  }
}