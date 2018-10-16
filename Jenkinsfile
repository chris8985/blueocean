pipeline {
  agent any
  stages {
    stage('add-job') {
      steps {
        build(job: 'first-free-job', propagate: true, quietPeriod: 1)
      }
    }
  }
}