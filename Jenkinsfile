#!/usr/bin/env groovy

def label = "tiagolabel"

podTemplate(label: label,
        containers: [
                containerTemplate(name: 'alpine', image: 'alpine:3.11', ttyEnabled: true, command: 'cat'),
        ],
        ) {
    node(label) {
        stage('Run shell') {
            container('alpine') {
                sh 'echo "hello world"'
            }
        }
    }
}
