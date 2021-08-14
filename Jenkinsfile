pipeline {
  agent any
  stages {
    stage('build') {
      agent {
        node {
          label 'fedora'
        }

      }
      steps {
        sh 'echo start'
        archiveArtifacts(artifacts: 'README.md', onlyIfSuccessful: true)
      }
    }

    stage('deploy') {
      agent {
        node {
          label 'ubuntu'
        }

      }
      steps {
        sh 'pwd'
      }
    }

  }
}