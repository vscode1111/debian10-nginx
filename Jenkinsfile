pipeline {
  agent any
  stages {
    stage('Nginx stop'){
      steps {
        timeout(time: 2, unit: 'MINUTES') {
          sh 'service nginx stop'
        }
      }
    }
    

    stage('Nginx start'){
      steps {
        timeout(time: 3, unit: 'MINUTES') {
          sh 'service nginx star'
        }
      }
    }
  }
}