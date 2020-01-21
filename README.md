# SettingWeb

An example project - Spring Web Project

## Getting Started

This project is an example of spring web application which can show movie list in DB.

### Setting Environment

```
JDK 1.8u231
Eclipse
    - STS Plugin(Spring Tools 3 Add-On for Spring Tools 4)
Apache Tomcat 9
    - Add the Tomcat server to the project
MariaDB 10.4.10
    - theater.movie(int id, String movie_name, String director, String types)
```

    pom.xml properties
        - check java-version
        - check springframework-version
    pom.xml plugin
        - check maven-compiler-plugin version
        - match source and target to java-version
    pom.xml dependency
        - mariadb-java-client
        - commons-dbcp
        - spring-jdbc
        - mybatis
        - mybatis-spring
        - log4jdbc-log4j2-jdbc4.1

### Issues

__Issue1__
    
    * Spring, MariaDB, Mybatis
        root-context.xml <context:component-scan> error
            solved: edit and add xmlns:context & xsi:schemaLocation
            
__Issue2__

    * setting path for controller
        http 404 error
            solved: build path - add webapp folder
        

### Example

![result](https://github.com/dianakoh/settingweb/blob/master/result.jpg)