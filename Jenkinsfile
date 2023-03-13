pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn build'
      }
    }

    stage('compile') {
      steps {
        sh 'mvn compile'
      }
    }

    stage('test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('package') {
      steps {
        sh 'mvn package'
      }
    }

  }
  environment {
    maven = 'maven-3.8.2'
  }
}
