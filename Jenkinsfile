library 'my-jenkins-lib'

pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Calling build'
        updateSubmodules(submodule: 'test-jenkins-repo')
        echo 'Called build'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
}
