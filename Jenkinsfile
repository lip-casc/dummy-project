#!/usr/bin/env groovy



pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'println "It's working !!!"'
            }
        }
    }
}
