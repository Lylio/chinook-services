![Java](https://github.com/Lylio/helper-repo/blob/master/img/logos/java.png)
![Spring Boot](https://github.com/Lylio/helper-repo/blob/master/img/logos/spring-boot.png)
![Chinook](https://github.com/Lylio/helper-repo/blob/master/img/logos/chinook.png)

# Chinook
## Spring Cloud Config Server: configuration server for microservice and web application properties.

https://chinook-server.herokuapp.com/application/default

### Docker Launch
to do
 
### Maven Launch
 Pass git credentials to JAR as system variables:
 1. mvn clean install
 2. cd target/
 3. java -jar chinook-0.0.1-SNAPSHOT.jar --git.username=username --git.password=password
 4. Verify the config has been pulled from https://github.com/Lylio/config-repo
at http://localhost:8888/application/default
