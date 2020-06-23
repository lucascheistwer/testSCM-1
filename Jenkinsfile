pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'git pull origin master'
        sh 'gradle build'
      }
    }

    stage('Test') {
      steps {
        echo 'Test'
      }
    }

    stage('Validate') {
      steps {
        echo 'Validate'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}