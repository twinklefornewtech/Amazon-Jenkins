pipeline {
  agent any
  stages {
    stage('compile ') {
      steps {
        buildMaven()
      }
    }
  }
  environment {
    PATH = '/usr/bin:/bin:/usr/local/bin'
  }
  post {
    success {
      echo 'Build success 1'
    }

    failure {
      echo 'Failure in the build'
    }

  }
}
