# CRUD App with Spring Boot

This is the code developed in the tutorial (https://stormpath.com/blog/tutorial-crud-spring-boot-20-minutes) on creating a flexible CRUD app with Spring Boot.

It features full REST compliance and an embedded database. This has the capability to load external jars.

### Requirements

- Maven
- JDK 7

### Running

To build and start the server simply type

```sh
$ mvn spring-boot:run
```
run: java -Dloader.path="jars/" -Dloader.home=/<path-to>/stormpath-spring-boot-jpa-example/ -Dloader.debug=true -jar target/demo-0.0.1-SNAPSHOT.jar

from the root directory.

### Using

You can see what urls are available using curl:

```sh
$ curl localhost:8080
```

You can view existing people objects using a similar request:

```sh
$ curl localhost:8080/persons
```

and can create new ones using a POST:

```sh
$ curl -X POST -H "Content-Type:application/json" -d '{ "firstName" : "Karl", "lastName" : "Penzhorn" }' localhost:8080/persons
```



### License
----

MIT

