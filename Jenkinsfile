pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''chmod +x mvnw
./mvnw package
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