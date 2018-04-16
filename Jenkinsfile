pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ls -la'
      }
    }
    stage('Test') {
      parallel {
        stage('test1') {
          steps {
            sh 'ls -la'
          }
        }
        stage('test2') {
          steps {
            sh 'uname -a'
          }
        }
      }
    }
    stage('report') {
      steps {
        sh 'pwd'
      }
    }
  }
}