pipeline {
  agent any
  stages {
    stage('Preperation') {
      steps {
        echo '.....Preparation.....'
      }
    }
    stage('Build') {
      steps {
        echo '.....Build.....'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sleep 5
          }
        }
        stage('Chrome') {
          steps {
            echo '.....Tested on Chrome.....'
          }
        }
        stage('Firefx') {
          steps {
            echo '.....Tested on Firefox.....'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo '.....Deploy.....'
      }
    }
  }
}