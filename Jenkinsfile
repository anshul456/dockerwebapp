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
        script {
           docker.image('node-app').withRun('-d=true -p 8888:8080')
          }
        }
      }
    stage('Remove Unused docker image') {
      steps{
        sh "docker rmi $registry:$BUILD_NUMBER"
      }
    }
  }
}
