pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/dhlee56/docker_jenkins_blueocean.git'
      }
    }

    stage('Build') {
      steps {
        tool 'maven3'
        sh 'maven3 spring-boot:run'
      }
    }

  }
}