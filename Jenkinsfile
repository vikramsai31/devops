pipeline {
  agent any
  stages {
    stage('Script run') {
      steps {
        sh 'aws s3 cp jenkins/starter-website.zip s3://test-webapp/starter-website.zip'
      }
    }
  }
}