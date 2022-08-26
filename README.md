# Jenkins Docker Compose

You can access the project through the following link: https://build.homelab.

## Config Files:

We added a help file with the default configuration to connect Jenkins and the OpenLDAP. Check the [ldap.txt](help/ldap.txt "ldap file") file.

## Folders:

1. Default folder.

``` bash
  /var/jenkins_home
```

2. Log folder.

``` bash
  /var/jenkins_home/log.properties
```

## Commands:

1. Enter the container.

``` bash
  docker exec -it jenkins bash
```

1. To install plugins.

``` bash
  /usr/local/bin/install-plugins.sh docker-slaves github-branch-source:1.8
  /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt
```

## Backup:

``` bash
  # The "." means the current folder.
  docker cp jenkins:/var/jenkins_home .  
```

## Restore:

``` bash
  # The "." means the current folder.
  docker cp . jenkins:/var/jenkins_home
```

## References:

1. [Jenkins no Docker Hub.](https://hub.docker.com/r/jenkins/jenkins "Jenkins no Docker Hub")

1. [Official Jenkins Docker image.](https://github.com/jenkinsci/docker/blob/master/README.md "Official Jenkins Docker image")

1. [Getting started with the Guided Tour.](https://jenkins.io/doc/pipeline/tour/getting-started/ "Getting started with the Guided Tour")

1. [Getting started with Blue Ocean.](https://jenkins.io/doc/book/blueocean/getting-started/ "Getting started with Blue Ocean")

1. [How to build a staging server with Docker, Jenkins and Traefik 1.](http://blog.francoisfaubert.com/2018/06/11/dockerized-jenkins-with-traefik.html "How to build a staging server with Docker, Jenkins and Traefik 1")

1. [How to build a staging server with Docker, Jenkins and Traefik 2.](http://blog.francoisfaubert.com/2018/06/11/dockerized-jenkins-with-traefik-2.html "How to build a staging server with Docker, Jenkins and Traefik 2")

1. [How to build a staging server with Docker, Jenkins and Traefik 3.](http://blog.francoisfaubert.com/2018/06/11/dockerized-jenkins-with-traefik-3.html "How to build a staging server with Docker, Jenkins and Traefik 3")

1. [How to build a staging server with Docker, Jenkins and Traefik 4.](http://blog.francoisfaubert.com/2018/06/11/dockerized-jenkins-with-traefik-4.html "How to build a staging server with Docker, Jenkins and Traefik 4")

1. [Traefik basics with Docker-Compose.](https://www.tikalk.com/posts/2017/10/10/traefik-basics-with-docker-compose/ "Traefik basics with Docker-Compose")
1. [Using environment variables (Get started with Jenkins, part 7).](https://www.youtube.com/watch?v=_t-hZTX97AI "Using environment variables (Get started with Jenkins, part 7)")

1. [Monitor disk usage (Get started with Jenkins, part 9).](https://www.youtube.com/watch?v=LMXdIE55rWo "Monitor disk usage (Get started with Jenkins, part 9)")

1. [Build status badges (Get started with Jenkins, part 10).](https://www.youtube.com/watch?v=clQEdNdOBm0 "Build status badges (Get started with Jenkins, part 10)")

## License:

[MIT](LICENSE "MIT License")

## Created by: 

1. Luciano Sampaio.
