pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Compile system') {
      steps {
        sh 'sh \'mvn package\''
      }
    }

  }
}