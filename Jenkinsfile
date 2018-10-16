pipeline {
  agent any
  stages {
    stage('scm') {
      steps {
        build(job: 'flow-build', quietPeriod: 1, wait: true)
      }
    }
  }
}