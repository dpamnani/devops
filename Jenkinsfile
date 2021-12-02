pipeline {
  agent any
  stages {
    stage('Build Jar') {
      steps {
        sh '''sudo -S <<< fenris
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"brew install maven
mvn -v
apt-get install maven
chmod +x mvnw
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