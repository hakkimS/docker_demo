
    pipeline {
    agent {
        docker {
              image 'maven:3.8.1-adoptopenjdk-11'
              label 'my-defined-label'
              alwayspull true
        }
    }
    stages {
        stage('Steps run inside docker here ...') {
            steps {
                sh "mvn --version"
            }
        }
    }
