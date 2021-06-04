#!/usr/bin/env groovy



podTemplate(label: tiagolabel,
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
