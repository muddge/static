pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        sh '''
                 echo "Multline shell steps works too"
                 ls -lah
                 '''
      }
    }

  }
}