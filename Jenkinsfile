pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(region:'us-east-1') {
          s3Upload(file:'index.html', bucket:'roy-udacity-jenkins-website', path:'target/index.html')              
        }
      } 
    } 
  } 
}
