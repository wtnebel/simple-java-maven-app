pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn compile'
        sh 'pwd'
        archiveArtifacts(allowEmptyArchive: true, artifacts: '**/target/*.jar')
      }
    }
  }
}