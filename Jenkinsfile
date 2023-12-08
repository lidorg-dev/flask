pipeline {
  agent {
    node {
      label 'centos-7-slave'
    }

  }
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/lidorg-dev/flask.git', branch: 'main', changelog: true, poll: true)
      }
    }

    stage('Build') {
      steps {
        sh 'echo "helllo"'
      }
    }

  }
}