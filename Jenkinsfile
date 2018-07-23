pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello world'
      }
    }
    stage('error') {
      steps {
        bat 'java -version'
        echo 'hello world'
      }
    }
  }
}