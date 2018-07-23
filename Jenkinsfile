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
        echo 'hello world'
      }
    }
  }
  environment {
    MY_NAME = 'chandan'
  }
}