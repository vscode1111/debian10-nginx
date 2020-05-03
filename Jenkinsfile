pipeline {
  agent any
  environment {
    HOME = '.'
  }
  stages {
    stage('Nginx stop'){
      steps {
        timeout(time: 2, unit: 'MINUTES') {
          sh 'npm -v'
        }
      }
    }

    stage('Nginx start'){
      steps {
        timeout(time: 3, unit: 'MINUTES') {
          sh 'npm -v'
        }
      }
    }
  }
}