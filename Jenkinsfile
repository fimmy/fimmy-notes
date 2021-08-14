pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo start'
        archiveArtifacts(artifacts: 'README.md', onlyIfSuccessful: true)
      }
    }

  }
}