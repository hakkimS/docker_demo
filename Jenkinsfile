pipeline{
    agent {
    docker {
        image 'maven:3.8.1-adoptopenjdk-11'
        label 'my-defined-label'
        args  '-v /tmp:/tmp'
        alwayspull true
    }
        
        stages{
        stage("pull")
            {
                steps{
                    script{
                    
                    def image = docker.image('lmaven:3.8.1-adoptopenjdk-11)
                   image.inside{
                   image.pull()
                  }
                    }
                
                }
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
