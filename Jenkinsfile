

node {
    checkout scm

    def fetchImage() {
  agent {
   docker {
    label “target_node ”
    image 'https://registry.hub.docker.com'
    alwaysPull true
    registryUrl 'https://registry.hub.docker.com’
    registryCredentialsId ‘docker-id’
   }
  }
}
    
    /*
    docker.withRegistry('https://registry.hub.docker.com/', 'docker-id') {
        
        def image = docker.image('luhqim/node-web-app')
        image.inside{
           image.pull() 
        alwaysPull false
                  }
        
    }
*/
}

