

node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', 'docker-id') {
        
        def maven = docker.image('luhqim/node-web-app')
        maven.inside{
           maven.pull()
        /* Push the container to the custom Registry */
        alwaysPull true
                  }
        
    }
}

