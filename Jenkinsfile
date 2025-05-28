pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', 'https://github.com/jindalmayank09/spring-batch-h2.git'
      }
    }
    stage('Build') {
      steps {
        echo 'Compiling code...'
      }
    }
    stage('Test') {
      steps {
        echo 'Running unit tests...'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying to staging environment...'
      }
    }
  }
}
