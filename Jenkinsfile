pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo start'
        archiveArtifacts(artifacts: 'test', onlyIfSuccessful: true)
      }
    }

  }
}