node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub_id') {

        def customImage = docker.build("hernanisoares/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}