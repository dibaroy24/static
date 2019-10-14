pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(region:'us-east-1', credentials:'IDofAwsCredentials') {
          s3Upload(file:'index.html', bucket:'roy-udacity-jenkins-website', path:'/index.html')
        }
      } 
    } 
  } 
}
