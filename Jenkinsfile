pipeline {
  agent any
  stages {
    stage('Script run') {
      steps {
        sh 'aws s3 jenkins/starter-website.zip cp s3://test-webapp/'
      }
    }
  }
}