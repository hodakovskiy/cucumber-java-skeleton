pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean verify'
      }
      post {
        always {
          cucumber '**/*.json'

        }

      }
    }
  }
}