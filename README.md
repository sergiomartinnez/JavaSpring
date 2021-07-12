# Java Spring

## Table of Contents
* [General info](#general-info) 
* [Technologies](#technologies) 
* [Setup](#setup)
* [Extra information](#Extra)

------------
## General info

In this course i learned about java Spring, his frameworks, his different projects and how it is helpful in simplification and creation of projects with less code. In the files you will find the project platzi market, a web for administration of markets and how to request information by query methods for a DB. In the project also you will find files and codelines for updating information and deleting as well. In the end you will find security codelines for protecting our information and DB from malwares, like interactions that requiere authentication. This project was divided in 3 layers: domain, persistance and web. 

Just for aclaration we use spanish classes because after in development and improving the code, we translate it into english version, it was necesary because the teacer said.

------------
## Technologies

>- OpenJDK11 (requieres installation)
>- IntelliJ IDEA (requieres installation)
>- PostgreSQL
>- SpringFramework

## Dependencies:

>- Spring Boot Starter Data JPA
>- PostgreSQL JDBC Driver
>- SpringFox Swagger2
>- Springfox Swagger UI
>- Spring Boot Starter Security
>- JSON Web Token Support For The JVM

------------
## Setup
This project was made on a Windows 10 OS.

### IntelliJ IDEA 
- Go to https://www.jetbrains.com/idea/download/ and download the Community version

### OpenJDK
- Go to https://adoptopenjdk.net/ and download the following version:
    - OpenJDK 11

###  PostgreSQL
- Go to https://www.enterprisedb.com/downloads/postgres-postgresql-downloads and click donwload PostgreSQL 11.12 for your OS.
- Complete installation process

###  SpringFramework
- Go to https://start.spring.io/ and select Gradle project and then click the genetere button
- Decompress the downloaded folder
- Open Intellij IDEA and open the build.gradle file within the downloaded folder


*Within Intellij IDEA*

### Spring Boot Starter Data JPA 
- Copy the next code and insert it into the build.graddle file in the dependencies part of the code.
-  `<!-- https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-starter-data-jpa -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
    <version>2.5.2</version>
</dependency>`


### PostgreSQL JDBC Driver
- Copy the next code and insert it into the build.graddle file in the dependencies part of the code.
- `runtimeOnly 'org.postgresql:postgresql'`

### SpringFox Swagger2
- Copy the next code and insert it into the build.graddle file in the dependencies part of the code.
- `implementation 'io.springfox:springfox-swagger2:2.9.2'`

### SpringFox Swagger UI
- Copy the next code and insert it into the build.graddle file in the dependencies part of the code.
- `implementation 'io.springfox:springfox-swagger-ui:2.9.2''`

### Spring Boot Starter Security
- Copy the next code and insert it into the build.graddle file in the dependencies part of the code.
- `implementation 'org.springframework.boot:spring-boot-starter-security:2.5.2'`

### JSON Web Token Support For The JVM
- Copy the next code and insert it into the build.graddle file in the dependencies part of the code.
- `implementation 'io.jsonwebtoken:jjwt:0.9.1'`


------------
## Extra

>- What spring is as framework
>- projects of spring (framework, boot, Data, Security)
>- Spring annotations
>- not use primitive type of data in Spring
>- only create the required relationships between entities for better App performance
>- save time using SpringData by performing databases operations without code
>- JPA annotations
>- use CrudRepository interface
>- Query methods
>- Data mapper pattern
>- Work with an existing table that is in another language using data mapper
>- dependency inyection
>- Make graphic documentatio for an API using Springfox Swagger
>- Make authentication required to certain API interactions
>- JSON web token
>- Manage certain level of security

------------
### commands that i learned
|  Command | Function  |
| ------------ | ------------ |
| @Springbootapplication | Tells Spring Boot that a class manages the app   |
| @Entitiy | Use in java class that it is representing a table in the database   |
| @table  | Receives the name of the table to which our class is mapping   |
| @column  | Used when the name of our column is different from the name of the attribute of our table   |
| @id  | Represents the primary key of the table |
| @EmbededId  | Represents the primary key of the table inside the class when is composite  |
| @GenerateValue  | Automatically generate values for the primary keys   |
| @OneToMany @ManyToOne  | Represent existing relationships in tables but represented in classes   |
| @Embeaddable   | Classes to embed other classes  |
| @Query    | Used to make native queries   |
| @Repository   | Tells the class that it interacts with the database |
| @Component   | Indicates a class is a spring component  |
| @Mapper   |   Used to map  |
| @Mappings()   | Indicates how we want to do the mapping  |
| @Mapping   | Indicates source and target to map if they have different names  |
| @InheritInverseConfiguration   | Indicates that the conversion we will perform is the inverse |
| @Autowired   | Spring manages objects that we haven't initialized creating them by itself  |
| @Service   | Indicates that a class is a business logic service  |
| @RestController   | Tells spring that a class will be a controller of a rest API |
| @RequestMapping | It indicates in which path it will accept the requests that we make |
| @PathVariable | Is to specify the path that you will put in the URL |
| @GetMapping    | To obtain information  |
| @Postmapping  | To save or update information  |
| @Deletemapping | To delete information |
| CrudRepository methods | save(), delete(), update() |
| @ApiOperation | is to add a description on the swagger page to the methods |
| @ApiResponse | is the way he responds |
| @ApiResponses | is to put togetjer some Apiresponse |

