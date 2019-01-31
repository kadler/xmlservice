pipeline {
  agent {
    node {
      label 'ibmi7.1'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'ls'
        sleep 5
      }
    }
    stage('unit test') {
      parallel {
        stage('unit test') {
          steps {
            sleep 10
          }
        }
        stage('function test') {
          steps {
            sleep 15
          }
        }
      }
    }
    stage('deploy') {
      steps {
        sleep 1
      }
    }
  }
}