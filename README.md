# Hello World Apache Wayang

This is a demo code to generate a project for using a Apache Wayang

# Compile Hello-World

To compile the code you need to have installed Java 11

```shell
./mvnw clean package 
```

# Running Hello-World

To run the Hello-World you need to execute the following command 

```shell
java \
    -cp $(pwd)/target/wayang-project-jar-with-dependencies.jar  \
    -Dwayang.configuration="file://$(pwd)/conf/wayang.properties" \
    -Dlog4j.configurationFile="file://$(pwd)/conf/log4j.properties" \
    HelloWorldAPIControl \
    spark file://$(pwd)/input/input.txt
```

or you can use the command

```shell
./bin/run.sh
```