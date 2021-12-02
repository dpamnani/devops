pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo -S <<< "fenris" mvn package
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