pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Compile system') {
      steps {
        sh '''def mvnhome= tool name: "maven-3",type: "maven"
sh "${mvnhome}/bin/mvn package"'''
      }
    }

  }
}