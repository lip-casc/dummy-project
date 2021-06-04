#!/usr/bin/env groovy

@Library(['github.com/indigo-dc/jenkins-pipeline-library@tree/release/2.1.0']) _

def projectConfig

pipeline {
  agent any
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
