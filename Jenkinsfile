pipeline {
  agent { docker 'gradle:7.4.2-jdk8' }
  stages {
    stage('Build') {
      steps {
        sh 'gradle clean build'
          junit 'build/test-results/**/TEST-*.xml'
        }
    }
    stage('deploy to staging') {
      steps {
        echo "deploying to staging"
      }
    }
    stage('deploy to production') {
      steps {
        echo "deploying to production"
      }
    }
  }
}