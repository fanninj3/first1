pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        parallel(
          "Dev": {
            build 'compile'
            
          },
          "test": {
            fileExists 'bla'
            
          }
        )
      }
    }
    stage('Test') {
      steps {
        sh '''high
'''
      }
    }
    stage('prepared') {
      steps {
        echo 'jiji'
      }
    }
  }
  environment {
    sampleEnv = 'dev'
  }
}