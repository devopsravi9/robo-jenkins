pipeline {
  agent any
  environment {
    URL = "google.com"
    SSH = credentials('SSH')
  }
  stages {
    stage ('test1') {
      steps {
        sh 'ls -al'
        sh ' echo ${URL} '
        sh ' echo ${SSH}'
        }
      }
    stage ('test2') {
      steps {
        sh 'echo hello world'
        }
      }
    }
  }

env.URL="google.com"
node {
  stage ('test1') {
    sh ' echo scripted approach'
    sh 'ceho ${ URL }'
     
    }
  }