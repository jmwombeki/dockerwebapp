node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        // def customImage = docker.build("my-image:${env.BUILD_ID}")
        def customImage = docker.build("jmwombeki/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
