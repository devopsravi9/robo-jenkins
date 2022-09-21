pipeline {
  agent any
  environment {
    MY_URL = "google.com"
    SSH = "credentials('SSH')"
  }
  stages {
    stage ('test1') {
      steps {
        sh 'ls -al'
        sh ' echo ${MY_URL} '
        sh ' echo ${SSH_USER}'
        }
      }
    stage ('test2') {
      steps {
        sh 'echo hello world'
        }
      }
    }
  }

env.MY_URL="google.com"
node {
  stage ('test1') {
    sh ' echo scripted approach'
    sh 'ceho ${ MY_URL }'
     
    }
  }