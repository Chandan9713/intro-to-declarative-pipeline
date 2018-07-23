pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}"
      }
    }
    stage('error') {
      steps {
        bat 'java -version'
        echo "Hello ${MY_NAME}"
      }
    }
  }
  environment {
    MY_NAME = 'chandan'
  }
}