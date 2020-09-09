pipeline {
  agent any
  stages {
    stage('Build') {
      post {
        success {
          junit '**/target/surefire-reports/TEST-*.xml'
          archiveArtifacts 'target/*.jar'
        }

      }
      steps {
        git 'https://github.com/stanmakori/simple-java-maven-app.git'
        sh 'mvn -Dmaven.test.failure.ignore=true clean package'
        archiveArtifacts(artifacts: 'target/*.jar', fingerprint: true)
      }
    }

    stage('Test') {
      steps {
        junit '**/surefire-reports/**/*.xml'
      }
    }

  }
  tools {
    maven 'M3'
  }
}