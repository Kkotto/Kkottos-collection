<nav>
  <h2>Contents</h2>
  <a href="#General">General</a>
  <ul>
    <li><a href="#Docker">Docker</a></li>
    <li><a href="#PostgreSQL">PostgreSQL</li>
  </ul>
</nav>

<h1 id="General">General</h1>
<h3 id="Docker">Docker</h3>
<ul>
  <li>Learn to build and deploy your distributed applications easily to the cloud with Docker: <a href=https://docker-curriculum.com/>Here.</a></li>
  <li>Intro to Docker with Java examples (YT video): <a href="https://youtu.be/FzwIs2jMESM?si=YAhEWU3jXL9XfNIp">Here.</a></li>
</ul>

> You can use the Spring Boot build plugins for Maven and Gradle to create container images. The plugins create an OCI image (the same format as one created by docker build) by using Cloud Native Buildpacks. ***You do not need a Dockerfile***, but you do need a Docker daemon, either locally (which is what you use when you build with docker) or remotely through the DOCKER_HOST environment variable. The default builder is optimized for Spring Boot applications, and the image is layered efficiently as in the examples above.
>
> Source: [Here](https://spring.io/guides/topicals/spring-boot-docker/)

compose.yaml
```
services:
  postgres:
    image: 'postgres:latest'
    environment:
      - 'POSTGRES_DB=DB_NAME'
      - 'POSTGRES_PASSWORD=PASSWORD'
      - 'POSTGRES_USER=USER'
    ports:
      - '5432'
```

<h3 id="PostgreSQL">PostgreSQL</h3>
<ul>
    <li>Using Postgres Effectively in Spring Boot Applications: <a href=https://hackernoon.com/using-postgres-effectively-in-spring-boot-applications>Here.</li>
    <li>Spring Boot, JPA/Hibernate, PostgreSQL CRUD example: <a href="https://www.bezkoder.com/spring-boot-postgresql-example/">Here.</a></li>
    <li>Конфигурационные параметры Hibernate: <a href="https://javarush.com/quests/lectures/questhibernate.level09.lecture04">Here.</a></li>
</ul>

```
spring.datasource.driver-class-name=org.postgresql.Driver
spring.datasource.url=jdbc:postgresql://localhost:5432/db_name
spring.datasource.username=username
spring.datasource.password=password
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.hibernate.ddl-auto=update
```
