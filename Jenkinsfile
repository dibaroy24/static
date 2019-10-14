pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(region:'us-east-1') {
          s3Upload acl: 'Private', bucket: 'roy-udacity-jenkins-website', cacheControl: '', excludePathPattern: '', file: 'index.html', includePathPattern: '', metadatas: [''], redirectLocation: '', sseAlgorithm: '', text: '', workingDir: ''              
        }
      } 
    } 
  } 
}
