# Annotations

## Learning Goals

- Provide a dictionary lookup of Spring Annotations.

## Introduction

This lesson is to provide a dictionary of all the annotations we have talked
about thus far in these lessons.

## Spring Annotations

Consider the following Spring Annotations:

| Annotation                 | Description                                                                                                               |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------|
| `@Autowired`               | Way to define link between beans in the Spring context                                                                    |
| `@Bean`                    | Annotation applied to methods to indicate that this object is to be added to the application context                      |
| `@Component`               | Stereotype annotation applied to classes to indicate that this object is to be added to the application context           |
| `@ComponentScan`           | Scan the package where the application is located for component classes (marked with `@Component`)                        |
| `@Configuration`           | Indicate that a class declares one or more `@Bean` methods                                                                |
| `@Controller`              | Specialization of the `@Component` annotation to indicate that a class is a controller                                    |
| `@EnableAutoConfiguration` | Enable Spring Boot's auto-configuration mechanism                                                                         |
| `@Indexed`                 | Indicates that all interfaces that extend the `Repository` interface should be treated as candidates for repository beans |
| `@PathVariable`            | Maps the dynamic path value to the parameter                                                                              |
| `@Repository`              | Specialization of the `@Component` annotation, to indicate a repository class                                             |
| `@RequestParam`            | Indicates that a method parameter should be bound to the web request as a parameter                                       |
| `@ResponseBody`            | Configures Spring to return a response from the controller methods                                                        |
| `@RestController`          | Combines the `@Controller` and `@ResponseBody` annotations                                                                |
| `@Scope`                   | Define the scope of a bean                                                                                                |
| `@Service`                 | Specialization of the `@Component` annotation, to indicate a service class                                                |
| `@SpringBootApplication`   | Combines the `@ComponentScan`, `@Configuration`, and `@EnableAutoConfiguration` annotations                               |

Consider the following Spring Mapping Annotations:

| Annotation        | Description                                                                                                  |
|-------------------|--------------------------------------------------------------------------------------------------------------|
| `@DeleteMapping`  | Shorthand for the `@RequestMapping(method=RequestMethod.DELETE)` annotation; Handles DELETE requests         |
| `@GetMapping`     | Shorthand for the `@RequestMapping(method=RequestMethod.GET)` annotation; Handles GET requests               |
| `@PostMapping`    | Shorthand for the `@RequestMapping(method=RequestMethod.POST)` annotation; Handles POST requests             |
| `@PutMapping`     | Shorthand for the `@RequestMapping(method=RequestMethod.PUT)` annotation; Handles PUT requests               |
| `@RequestMapping` | Annotation for mapping web requests onto methods in request-handling classes with flexible method signatures |

Consider the following Spring Validation Annotations:

| Annotation   | Description                                                                                                                                          |
|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| `@Max`       | Define the upper boundary of numeric values                                                                                                          |
| `@Min`       | Define the lower boundary of numeric values                                                                                                          |
| `@NotBlank`  | Ensures a field is not empty, even after trimming                                                                                                    |
| `@NotEmpty`  | Ensures a field is not `null` and its length is greater than 0                                                                                       |
| `@NotNull`   | Ensures a field is not `null`                                                                                                                        |
| `@Pattern`   | Validates against a field against a regular expression                                                                                               |
| `@Size`      | Takes `min` and `max` parameters to define the length of a `String` or number of elements in a `Collection`                                          |
| `@Valid`     | This annotation is added before a controller method parameter to check if the field is valid against the field annotations                           |
| `@Validated` | This annotation is applied to a controller class to enable validation annotations for all parameters marked with `@PathVariable` and `@RequestParam` |

## Lombok Annotations

Consider the following Lombok Annotations:

| Annotation                 | Description                                                                                                                                              |
|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| `@AllArgsConstructor`      | Creates a constructor with all the fields taken in as arguments at compile-time                                                                          |
| `@NoArgsConstructor`       | Creates a constructor with no arguments at compile-time                                                                                                  |
| `@RequiredArgsConstructor` | Creates a constructor with 1 parameter for each field that requires special handling                                                                     |
| `@Getter`                  | Creates an accessor method for the field and/or every field defined in the class depending if the annotation is placed at the field level or class level |
| `@Setter`                  | Creates a mutator method for the field and/or every field defined in the class depending if the annotation is placed at the field level or class level   |
| `@EqualsAndHashCode`       | Creates an `equals()` and `hashCode()` method for the class at compile-time                                                                              |
| `@ToString`                | Creates a `toString()` method for the class at compile-time                                                                                              |
| `@Data`                    | Combines the `@RequiredArgsConstructor`, `@Getter`, `@Setter`, `@EqualsAndHashCode` and `@ToString` annotations                                          |

## JPA Annotations

Consider the following JPA Annotations:

| Annotation        | Description                                                                                          |
|-------------------|------------------------------------------------------------------------------------------------------|
| `@Entity`         | Defines the class as an entity; represents a table stored in a database                              |
| `@Column`         | Specifies the mapped column for a persistent property or field                                       |
| `@GeneratedValue` | Applied in conjunction with the `@Id` annotation and provides generation strategies for primary keys |
| `@Id`             | Defines the field as the primary key                                                                 |
| `@Table`          | Specifies the primary table for the annotated entity                                                 |
| `@Query`          | Defines a custom JPQL or native query                                                                |

## Resources

- [Configuration Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/context/annotation/Configuration.html)
- [Bean Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/context/annotation/Bean.html)
- [Component Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/stereotype/Component.html)
- [ComponentScan Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/context/annotation/ComponentScan.html)
- [Service Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/stereotype/Service.html)
- [Controller Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/stereotype/Controller.html)
- [SpringBootApplication Annotation](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/using-boot-using-springbootapplication-annotation.html)
- [Auto-configuration Documentation](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/using-boot-auto-configuration.html)
- [RestController Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/RestController.html)
- [GetMapping Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/GetMapping.html)
- [RequestParam Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/RequestParam.html)
- [ResponseBody Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/ResponseBody.html)
- [RequestMapping Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/RequestMapping.html)
- [Autowired Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/beans/factory/annotation/Autowired.html)
- [PathVariable Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/PathVariable.html)
- [BeanScope Documentation](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans-factory-scopes)
- [PostMapping Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/PostMapping.html)
- [Lombok Features Documentation](https://projectlombok.org/features/)
- [Indexed Annotation](https://docs.spring.io/spring-framework/docs/5.3.22/javadoc-api/org/springframework/stereotype/Indexed.html?is-external=true)
- [Repository Annotation Documentation](https://docs.spring.io/spring-data/commons/docs/current/api/org/springframework/data/repository/Repository.html)
- [PutMapping Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/PutMapping.html)
- [DeleteMapping Annotation](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/DeleteMapping.html)
- [Using @Query Documentation](https://docs.spring.io/spring-data/jpa/docs/current/reference/html/#jpa.query-methods.at-query)