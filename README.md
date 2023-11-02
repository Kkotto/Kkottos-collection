<nav>
  <h2>Contents</h2>
  <ul>
    <li><a href="#Docker-1">Docker</a></li>
  </ul>
</nav>

<h3 id="Docker-1">Docker</h3>
<ul>
  <li>Learn to build and deploy your distributed applications easily to the cloud with Docker: <a href=https://docker-curriculum.com/>Here.</a></li>
  <li>Intro to Docker with Java examples (YT video): <a href="https://youtu.be/FzwIs2jMESM?si=YAhEWU3jXL9XfNIp">Here.</a></li>
</ul>

> You can use the Spring Boot build plugins for Maven and Gradle to create container images. The plugins create an OCI image (the same format as one created by docker build) by using Cloud Native Buildpacks. ***You do not need a Dockerfile***, but you do need a Docker daemon, either locally (which is what you use when you build with docker) or remotely through the DOCKER_HOST environment variable. The default builder is optimized for Spring Boot applications, and the image is layered efficiently as in the examples above.
>
> Source: [Here](https://spring.io/guides/topicals/spring-boot-docker/)
