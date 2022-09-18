pipeline {
  agent {
    node {
      label 'node01'
    }

  }
  stages {
    stage('Log Ant version info') {
      steps {
        sh 'ant -version'
      }
    }

    stage('Build Ant ') {
      steps {
        sh 'ant clean compile test package war'
      }
    }

  }
}