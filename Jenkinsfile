pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello World!!!'
        echo "Hello ${params.Name}!"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Saraniya'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}