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

    stage('Github Jenkins Ant Build') {
      steps {
        git(url: 'https://github.com/Devops-self-training/jenkins_series-helloworld-java-ant', branch: 'jenkins-ci', changelog: true, credentialsId: 'coursera_lab')
      }
    }

  }
}