pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Calling build'
        build(
          job: 'test-jenkins-repo-submodules',
          parameters: [
            string(name: 'submodules', value: 'test-jenkins-repo')
          ],
          propagate: true,
          wait: true
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
