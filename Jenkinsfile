pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'Jenkins', region:'us-east-2'){
        s3Upload(file:'index.html', bucket:'udacity-muddge-project-4', path:'https://github.com/muddge/static/index.html')
        }
      }
    }
  }
}
