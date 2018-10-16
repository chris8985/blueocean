pipeline {
  agent any
  stages {
    stage('scm') {
      steps {
        build(job: 'flow-build', quietPeriod: 1, wait: true)
      }
    }
    stage('add-job') {
      steps {
        build(job: 'first-free-job', propagate: true, quietPeriod: 1)
      }
    }
  }
}