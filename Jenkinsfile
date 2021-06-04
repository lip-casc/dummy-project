#!/usr/bin/env groovy

def label = "tiagolabel"

podTemplate(label: label,
        containers: [
                containerTemplate(name: 'alpine', image: 'alpine:3.11', ttyEnabled: true, command: 'cat'),
        ],
        ) {
    node(label) {
            stages {
                stage('Run shell') {
                    container('alpine') {
                        sh 'echo "hello world"'
                    }
                }
            }
            post { 
                always { 
                    echo 'I will always say Hello again!'
                }
            }
    }
}
