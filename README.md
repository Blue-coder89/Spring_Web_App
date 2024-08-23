# Steps for running the maven project:

1) Pull the docker image of mysql from docker hub using the following command:
```docker pull mysql```
2) Run the docker image of mysql in a container using the following command:
```docker run -d -e MYSQL_ROOT_PASSWORD=secret -e MYSQL_DATABASE=taskdb --name mysqldb -p 3307:3306 mysql```

3) Check pom.xml for the dependencies required for the project like version of Java,maven etc. Make sure your system has the required versions of Java and maven installed.

4) Run the following command to build the project:
```mvn clean install```

5) Run the following command to build the project:
```mvn package```
6) Run the following command to run the project:
```mvn spring-boot:run```

7) Use postman to test the APIs.