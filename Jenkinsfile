node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/', '80081837') {

        def customImage = docker.build("yash/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
