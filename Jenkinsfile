pipeline {
  agent any
  stages {
    stage('SCM Checkout') {
      steps {
        sh 'git clone \'https://github.com/stanmakori/simple-java-maven-app.git\''
      }
    }

    stage('Compile Package') {
      steps {
        sh 'sh \'mvn package\''
      }
    }

  }
}