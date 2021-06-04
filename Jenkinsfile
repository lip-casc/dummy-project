#!/usr/bin/env groovy


pipeline {
  agent { label 'tiagolabel' }
  stages {
    stage('HelloWorld1') {
      steps {
        echo 'Hello from stage \"HelloWorld1\"'
      }
    }
    stage('HelloWorld2') {
      steps {
        echo 'Hello from stage \"HelloWorld2\"'
      }
    }
  }
}
