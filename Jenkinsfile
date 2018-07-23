pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello world'
      }
    }
    stage('error') {
      steps {
        bat 'java -version'
      }
    }
  }
}