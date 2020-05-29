pipeline {
  environment {
    registry = "4639345/docker-node"
    registryCredential = 'dockerHub'
    dockerImage = ''
  }
  agent any
  stages {
    stage('Building image') {
      steps{
        script {
          dockerImage = docker.build("node-app")
        }
      }
    }
    stage('Run Image') {
      steps{
          sh "docker run --rm -p 49160:8080 node-app"
        }
      }
  }
}
