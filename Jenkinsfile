

node {
    checkout scm
   
    docker {
    label “target_node ”
    image 'luhqim/node-web-app'
    alwaysPull true
    //registryUrl "https://registry.hub.docker.com"
    registryCredentialsId ‘docker-id’
   }

    
    
    docker.withRegistry('https://registry.hub.docker.com/', 'docker-id') {
        
        def image = docker.image('luhqim/node-web-app')
        image.inside{
           image.pull() 
                  }
        
    }
}

