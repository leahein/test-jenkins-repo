pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Calling build'
        build(
          job: '../test-jenkins-repo-submodules',
          propagate: true,
          wait: false
        )
        echo 'Called build'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
}
