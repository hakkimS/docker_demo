
    pipeline {
    agent {
        docker {
             registryCredentialsId   'docker-id'
            registryUrl             'https://registry.hub.docker.com/'
            image                   'luhqim/node-web-app'
            alwaysPull                true
        }
    }
    stages {
        stage('Steps run inside docker here ...') {
            steps {
                sh "docker ps"
            }
        }
    }
    }

/*
node {
    checkout scm
   
  
    docker.withRegistry('https://registry.hub.docker.com/', 'docker-id') {
        
        def image = docker.image('luhqim/node-web-app')
        image.inside{
           image.pull()
                  }
        
    }
    }
                              */
