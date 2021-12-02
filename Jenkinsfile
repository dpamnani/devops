pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo -S <<< "fenris" ./mvnw package
'''
        stash 'Target'
      }
    }

    stage('Execute .jar') {
      steps {
        unstash 'Target'
        sh 'java -jar Target/*.jar'
      }
    }

  }
}