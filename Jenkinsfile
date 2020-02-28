pipeline {
  agent any
  stages {
    stage('Lint HTML') {
      steps {
         sh 'tidy -q -e /var/lib/jenkins/workspace/static_master/index.html'
        }
      }
     stage('Upload to AWS') {
      steps {
        withAWS(credentials:'63d5838b-2571-434a-88ee-f5880182dc18', region:'us-east-2'){
        s3Upload(file:'index.html', bucket:'udacity-muddge-project-4')
        }
      }
    }
  }
 }
