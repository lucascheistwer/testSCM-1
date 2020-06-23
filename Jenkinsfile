pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'git pull origin master'
        bat 'gradlew.bat :spotlessApply'
        bat 'gradle build'
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

    stage('Analyze') {
      steps {
        bat 'gradle sonarqube'
      }
    }

    stage('Test Report') {
      steps {
        bat 'gradlew -i test jacocoTestReport'
      }
    }

  }
}
