pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Compile system') {
      steps {
        sh 'sh \'/tmp/maven363/bin/mvn package\''
      }
    }

  }
}