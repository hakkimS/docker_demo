

node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', 'docker-id') {
        
        def image = docker.image('luhqim/node-web-app')
        image.inside{
           image.pull()
        /* Push the container to the custom Registry */
        alwaysPull false
                  }
        
    }
}

