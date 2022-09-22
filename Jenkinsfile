//pipeline {
//  agent any
//  environment {
//    MY_URL = "google.com"
//    SSH = credentials('SSH')
//  }
//  stages {
//    stage ('test1') {
//      steps {
//        sh 'ls -al'
//        sh ' echo ${MY_URL} '
//        sh ' echo ${SSH}'
//        }
//      }
//    stage ('test2') {
//      steps {
//        sh 'echo hello world'
//        }
//      }
//    }
//  }
//
//env.MY_URL="google.com"
//node {
//  stage ('test1') {
//    echo " ${ MY_URL }"
//    }
//  }

pipeline {
  agent any
  options {
    ansiColor('xterm')
    }
  stages {
    stage ('create jenkins job') {
      steps {
        sh 'ansible-playbook jenkins.yml -e ansible_user=centos -e ansible-password=DevOps321'
        }
      }
    }
  }

