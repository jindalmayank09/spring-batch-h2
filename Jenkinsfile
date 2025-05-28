pipeline {
  agent any

  parameters {
    string(name: 'ENV', defaultValue: 'dev', description: 'Environment to deploy')
  }
  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', url: 'https://github.com/jindalmayank09/spring-batch-h2.git'
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
  post {
    success {
      echo 'Build succeeded!'
    }
    failure {
      echo 'Build failed!'
    }
    always {
      echo 'Job finished (success or fail)'
    }
  }
}
