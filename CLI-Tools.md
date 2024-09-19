# Java CLI Tools
sd
There are many cli tools in the java ecosystem, but I've broken them down into five categories that are relevant to my backend Java development:

1) Java Runtime and SDKwee
2) Build Tools & Dependency Management
4) Testing Tools
5) Spring Framework

Let's go deeper into each one!

<br/>

--

## Java Runtime and SDK CLI Tools

#### Java
Once you have installed Java on your machine, you should then have the `java` command available.

Use the `-version` flag to find out your current Java version.
```bash
java -version
```

#### Jabba
If you need to switch between multiple Java versions there are toold like [Jabba](https://github.com/shyiko/jabba) to make this relatively painless. 👍
```bash
jabba install zulu@~1.6.97
jabba use zulu@~1.6.97
```

--

## Build Tools

These cli tools take your application and turn them into a finished _jar_ or _war_ file. The only two really worth mentioning today are _maven_ and _gradle_ so those are the only two I'll mention here.

#### Maven
// TODO

#### Gradle
// TODO

--

## Testing Tools

Many types of tests...

#### Unit Tests With JUnit
// TODO

#### Code Coverage JUnit Tests With _____
// TODO

#### Mutation Tests With PITtest
// TODO

#### End-To-End API Testing With RestAssured
// TODO

#### Load Testing With JMeter
// TODO

#### Load Testing With Gatling
// TODO

--

## Spring CLI

Spring is a framework that models backend development with an MVC architecture. "Spring Boot" refers to the spring cli and _starters_ that allow developers to "boot up" new spring projects quickly and easily.

