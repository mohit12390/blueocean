pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'pwd && date'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'Hello world'
          }
        }

        stage('compile') {
          steps {
            sleep 3
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sh 'This is deploy'
      }
    }

  }
  environment {
    Name = 'mohit123'
    Age = '23'
  }
}