# Training Spring Boot

## 🚀 Start
An initial spring-boot project

- On StartAplication.java is added a method **hello()**
- Designed to take a String parameter called name

#### 📝Annotations

**@RestController** Tells Spring that this code describes an endpoint that should be made available over the web

**@GetMapping("hello")** Tells Spring to use our hello() method to answer requests that get sent to the http://localhost:8080/hello address

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

