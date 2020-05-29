node {
    checkout scm
    docker.withRegistery("https://registry.hub.docker.com","dockerHub"){
    def customImage = docker.build("node-app")
    customImage.push()
}

