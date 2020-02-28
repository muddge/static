pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'63d5838b-2571-434a-88ee-f5880182dc18', region:'us-east-2'){
        s3Upload(file:'index.html', bucket:'udacity-muddge-project-4', path:'https://github.com/muddge/static/index.html')
        }
      }
    }
  }
}
