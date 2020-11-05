![](https://github.com/Lylio/image-repo/blob/master/logos/java.png?raw=true)
![](https://github.com/Lylio/image-repo/blob/master/logos/spring-boot.png?raw=true)
![](https://github.com/Lylio/image-repo/blob/master/logos/chinook.png?raw=true)

# Chinook-Services
## Spring Cloud Config Server
### Description
A centralised configuration server for microservice and web application properties. Demo available at https://chinook-server.herokuapp.com/application/default

### Docker Launch
1. `docker build -t chinook-services .`
2. `docker run -e GIT_USERNAME={username} -e GIT_PASSWORD={password} -p 8888:8888 chinook-services:latest`
3. Verify the config has been pulled at http://localhost:8888/application/default
4. A different config file can be pulled with http://localhost:8888/<application name>/default
e.g http://localhost:8888/chatty-services/default
 
### Maven Launch
 1. `mvn clean install`
 2. `cd target/`
 3. `java -jar chinook-services-0.0.1-SNAPSHOT.jar --git.username={username} --git.password={password}`
 4. A different config file can be pulled with http://localhost:8888/insert-application/default
 e.g http://localhost:8888/chatty-services/default
