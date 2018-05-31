pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '/home/sergey/netbeans-8.2/java/maven/bin/mvn -Dtest=*Test test-compile surefire:test'
      }
      post {
        always {
          cucumber '**/*.json'

        }

      }
    }
  }
}