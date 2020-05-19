node {

    checkout scm

    docker.withRegistry('https://hub.docker.com/repositories', 'DockerHub') {

        def customImage = docker.build("ileaandrei/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
