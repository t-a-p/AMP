pipeline {
  agent any
  stages {
    stage('Prepare') {
      parallel {
        stage('Prepare') {
          steps {
            sh 'echo "From jenkinsFile"'
          }
        }
        stage('') {
          steps {
            build(job: '_MyJob', propagate: true)
          }
        }
      }
    }
  }
}