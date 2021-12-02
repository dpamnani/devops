pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''cd spring-petclinic-main
mvn package'''
        stash 'Target'
      }
    }

  }
}