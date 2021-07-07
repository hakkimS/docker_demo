

node {
    checkout scm

    docker.withRegistry('https://registry.docker.com', 'docker-id') {
        docker.pull("luhqim/node-web-app")
        /* Push the container to the custom Registry */
        alwaysPull true
    }
}

