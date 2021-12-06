pipeline {
  agent any
  stages {
    stage('build jar') {
      steps {
        sh '''ls
pwd
mvn package -e'''
      }
    }

  }
}