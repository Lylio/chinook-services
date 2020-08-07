![](https://github.com/Lylio/helper-repo/blob/master/img/logos/java.png?raw=true)
![](https://github.com/Lylio/helper-repo/blob/master/img/logos/spring-boot.png?raw=true)
![](https://github.com/Lylio/helper-repo/blob/master/img/logos/chinook.png?raw=true)

# Chinook
## Spring Cloud Config Server
### Description
A centralised configuration server for microservice and web application properties. Demo available at https://chinook-server.herokuapp.com/application/default

### Docker Launch
1. `docker build -t chinook .`
2. `docker run -e GIT_USERNAME={username} -e GIT_PASSWORD={password} -p 5555:8888 chinook:latest`
3. Verify the config has been pulled at http://localhost:5555/application/default
 
### Maven Launch
 1. `mvn clean install`
 2. `cd target/`
 3. `java -jar chinook-0.0.1-SNAPSHOT.jar --git.username={username} --git.password={password}`
 4. Verify the config has been pulled at http://localhost:8888/application/default
