pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Calling build'
        build(
          job: 'chabeja',
          propagate: true,
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
