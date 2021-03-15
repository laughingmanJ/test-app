podTemplate(containers: [
    containerTemplate(name: 'node', image: 'node:14-alpine', ttyEnabled: true, command: 'cat')
  ]) {

    node(POD_LABEL) {
        stage('Build') {
            container('node'){
                sh 'node --version'
            }
        }
    }
  }
