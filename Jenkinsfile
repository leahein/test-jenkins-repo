pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Calling build'
        build(
          job: "../test-jenkins-repo-submodules/master",
          parameters: [
            string(name: 'test_submodule', value: 'test-jenkins-repo')
          ],
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
