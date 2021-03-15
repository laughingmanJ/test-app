podTemplate(containers: [
    containerTemplate(name: 'node', image: 'node:14-alpine', ttyEnabled: true, command: 'cat')
  ]) {

    node(POD_LABEL) {
        try{
            stage('Build') {
                container('node'){
                    sh 'node --version'
                }
            }
        }
        catch(ex){
            println "Failed"
            throw(ex)
        }
    }
  }
