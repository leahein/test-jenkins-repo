pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Calling build'
        result = build(
          job: "../test-jenkins-repo-submodules/master",
          propagate: true,
        ).result
        echo "${result}"
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
