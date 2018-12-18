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
        stage('Test') {
          steps {
            sh 'echo "Inside Test"'
          }
        }
      }
    }
    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            sleep 10
          }
        }
        stage('Deploy2') {
          steps {
            sh 'echo "Inside Deploy2"'
          }
        }
        stage('Deploy3') {
          steps {
            sleep 30
          }
        }
      }
    }
    stage('Publish') {
      steps {
        sh 'echo "Publish the report"'
        sleep 50
      }
    }
  }
}