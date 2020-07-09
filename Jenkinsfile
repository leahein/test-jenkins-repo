library 'my-jenkins-lib'

pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Calling downstream'
        updateSubmodules(submodule: 'test-jenkins-repo')
        echo 'Called downstream'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
}
