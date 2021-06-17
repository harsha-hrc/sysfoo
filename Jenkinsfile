pipeline {
  agent none
  stages {
    stage('build') {
      steps {
        sh 'mvn compile'
        echo 'compile maven app'
      }
    }

    stage('test') {
      steps {
        echo 'test maven app'
        sh 'mvn clean test'
      }
    }

    stage('package') {
      steps {
        echo 'package maven app'
        sh 'mvn package -DskipTests'
      }
    }

  }
}