pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000 -v /var/jenkins_home:/var/jenkins_home'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }
  }
}