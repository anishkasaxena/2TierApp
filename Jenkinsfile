pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker { image 'python:3.9.19-alpine3.20' }

      }
      steps {
        sh 'mvn --version'
      }
    }

    
    stage('Front-end') {
      agent {
        docker { image 'node:16-alpine' }
      }
      steps {
        sh 'node --version'
      }
    }
  }
}