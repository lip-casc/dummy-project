#!/usr/bin/env groovy

def label = "k8sagent-e2e"

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
