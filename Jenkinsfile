pipeline {
  agent {
    node {
      label 'centos-7-slave'
    }

  }
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/lidorg-dev/flask.git', branch: 'main', poll: true, changelog: true)
      }
    }

    stage('Build') {
      steps {
        sh '''echo "hello"
echo "lidor"'''
      }
    }

    stage('Test') {
      steps {
        sh 'echo "hello"'
      }
    }

    stage('Package') {
      steps {
        echo 'hello'
      }
    }

  }
}