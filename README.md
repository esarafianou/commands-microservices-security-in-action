# Commands for the Microservices Security in Action book

## Container Usage

To run the examples within a container:

* Go into the sample's code, e.g. `cd [samples]/chapter02/sample01`
* Build the docker image from the Dockerfile: `docker build .`
* `docker run -it -p 8080:8080 <IMAGE_ID> /bin/bash` 
* Follow the book instructions:
    * `mvn clean install`
    * `mvn spring-boot:run`
