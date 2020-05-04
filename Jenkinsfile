pipeline {
  agent any
  stages {
    stage('Nginx stop'){
      steps {
        timeout(time: 1, unit: 'MINUTES') {
          sh 'service nginx stop'
        }
      }
    } 

    stage('Copy configs'){
      steps {
        timeout(time: 1, unit: 'MINUTES') {
          sh 'cp -r /var/lib/jenkins/workspace/debian10-nginx/conf.d /etc/nginx'
          sh 'cp -r /var/lib/jenkins/workspace/debian10-nginx/certs /etc/nginx'
        }
      }
    }  
    
    stage('Nginx start'){
      steps {
        timeout(time: 1, unit: 'MINUTES') {
          sh 'service nginx start'
        }
      }
    }
  }
}