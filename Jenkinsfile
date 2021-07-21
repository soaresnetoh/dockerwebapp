node {

    checkout scm
    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub_id') {
    def customImage = docker.build("hernanisoares/dockerwebapp:${env.BUILD_ID}")
        /* Push the container to the custom Registry */
        customImage.push()
        customImage.push('latest')
    }
}