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
            sh 'echo $name1'
          }
        }
        stage('deploy2') {
          steps {
            sh 'echo $name2'
          }
        }
      }
    }
    stage('final') {
      steps {
        sh 'echo "final"'
      }
    }
    stage('next') {
      steps {
        sh 'echo "bye"'
      }
    }
  }
  environment {
    name1 = 'joy'
    name2 = 'chan'
  }
}