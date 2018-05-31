pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn test'
      }
      post {
        always {
          cucumber '**/*.json'

        }

      }
    }
  }
}