# Project Info

This is spring cloud server which provides configuration to other projects using spring cloud client.

- Create a github repository
- Put client project properties file in github repository in the format:
 

    client-project-env.properties

    example: 
        limits-service.properties, 
        limits-service-dev.properties, 
        limits-service-qa.properties

- Github repository can be added to spring cloud server project in two ways:

  1. By adding a local github folder
  2. By adding github url
  
Example:

    spring.cloud.config.server.git.uri=file:///c:\\Users\\username\\microservice-local-git-repo
    OR
    spring.cloud.config.server.git.uri=https://github.com/username/microservice-local-git-repo.git