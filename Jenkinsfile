pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${params.Name}!"
      }
    }
    stage('error') {
      steps {
        bat 'java -version'
        echo "Hello ${params.Name}!"
      }
    }
    stage('Deploy') {
      options {
        timeout(time: 30, unit: 'SECONDS')
      }
      steps {
        input 'should we countinue ?'
        echo 'continue with deployment'
      }
    }
  }
  environment {
    MY_NAME = 'chandan'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}