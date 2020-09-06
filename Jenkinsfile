pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Package app') {
      steps {
        sh 'sh "${mvn} package"'
      }
    }

  }
}