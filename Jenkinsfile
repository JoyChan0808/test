pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh 'echo "test"'
      }
    }
    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            sh 'echo "deploy 1"'
          }
        }
        stage('deploy2') {
          steps {
            sh 'echo "deploy2"'
          }
        }
      }
    }
    stage('final') {
      steps {
        sh 'echo "final"'
      }
    }
  }
}