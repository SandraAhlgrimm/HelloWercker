# hello_world
SpringBoot, Gradle, Docker, Wercker

[![wercker status](https://app.wercker.com/status/f2e4c13fd194cde02c47337ea5da6baa/m "wercker status")](https://app.wercker.com/project/bykey/f2e4c13fd194cde02c47337ea5da6baa)



## runs with Dockerfile

        ./gradlew build buildDocker
        
       docker run -p 8080:8080 name


## runs with wercker
        add this repository to http://app.wercker.com/
            save your docker login in the project settings/ Environment variables as DOCKER_USER and DOCKER_PASSWORD
            the rest is wercker doing for you
        pull the latest docker image with e.g.: docker pull sandra/hello_world:latest
        run the dockerfile: docker run -p 8080:8080 sandra/hello_world:latest
        
To check the Application in your Browser you can find the IP the docker machine is currently running at with

        docker-machine ip
      
        ![Screenshot](/screenshot.png)
        
## Tutorials


        https://spring.io/guides/gs/gradle/

        https://spring.io/guides/gs/spring-boot-docker/
        
        wercker.yml https://github.com/mihkels/box-java8-oracle
