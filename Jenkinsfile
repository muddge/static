pipeline {
  agent any
  stages {
    stage('Uploiad to AWS') {
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
