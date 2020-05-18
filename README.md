# Training Spring Boot

## 🚀 Start
An initial spring-boot project

- On StartAplication.java is added a method **hello()**
- Designed to take a String parameter called name

#### 📝Annotations

**@RestController** Tells Spring that this code describes an endpoint that should be made available over the web

**@GetMapping("/hello")** Tells Spring to use our hello() method to answer requests that get sent to the http://localhost:8080/hello address

**@RequestParam** Is telling Spring to expect a name value in the request, but if it’s not there, it will use the word “World” by default

#### 🤸Try it

> in the project directory
>
> ./mvnw spring-boot:run
>
> visit http://localhost:8080/hello
>
> to the end of the URL add ?name=YourName
>

-----------------------------------------------

## 🚀 Jpa

An initial project of build an application that uses Spring Data JPA to store and retrieve data in a relational database.

- The application stores **Customer** POJOs (Plain Object Java Objects) in a memory-based database

##### Dependencies

- Spring Data JPA

- H2 Database

#### 📝Annotations

#### Customer

**@Entity** indicate that is a JPA entity. Because **@Table** annotation exist, it is assumed that this entity is mapped to a table with class name.

**@Id** recognize it is a object's ID.

**@GeneratedValue** to indicate that the ID should be generated automatically.

Porperties **unannotated** is assumed that they are mapped to columns that share the same names as the properties themselves.

--------------------------------------------------------------
#### CustomerRepository

**CrudRepository** interface has inherits several methods for working with object persitence. Also lets you define other query methods by declaring their method signature. 

---------------------------------------------------------------

#### SpringBootApplication

**@SpringBootApplication** annotation that adds all of the following:

**@Configuration** Tags the class as a source of bean definitions for the application context.

**@EnableAutoConfiguration** Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings.

**@ComponentScan**  Tells Spring to look for other components, configurations, and services in the com/example package, letting it find the controllers.

**@Bean** Automatically runs the code when the application launches.

**@EnableJpaRepositories(basePackageClasses=MyRepository.class)** You can point out alternate packages by using.

#### 🤸Try it

> in the project directory
>
> ./mvnw spring-boot:run



