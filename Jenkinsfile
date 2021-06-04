#!/usr/bin/env groovy



pipeline {
    agent { docker { image 'python:3.6' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                println "It's working !!!"
            }
        }
    }
}
