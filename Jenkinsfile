pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn compile'
        archiveArtifacts(allowEmptyArchive: true, artifacts: '**/target/*.jar')
      }
    }
  }
}