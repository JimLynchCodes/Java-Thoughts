# Java Code Coverage Reports With JaCoCo

Code coverage reports show you _code that has not been executed during by your suite of unit tests!_

[JavaCoCo](https://www.eclemma.org/jacoco/) is a popular tool in the Java ecosystem for easily generating nice code coverage reports. 

<br/>

## Adding Code Coverage To An Existing Gradle Project

Make these two changes to your `build.gradle` file:

<br/>

1) Add `id 'jacoco'` to the plugins section: 

```groovy
plugins {
    id "java"
    id 'jacoco'
}
```

<br/>

2) At the bottom of the file add this block of groovy configuration code:

```groovy
jacocoTestReport {
    reports {
        xml.required = false
        csv.required = false
        html.outputLocation = layout.buildDirectory.dir('jacocoHtml')
    }
}
```

<br/>

Then run the command to generate the report: 
```bash
gradle build jacocoTestReport
```

<br/>

View the report by opening the `/build/jacocoHtml/index.html` file in your browser.

---

<br/>

## JavaCoCo HTML Report Screenshots

<br/>

Directory:
<img src="https://github.com/JimLynchCodes/Java-Thoughts/blob/main/JavaCoCo-directory.png"/>

<br/>

Java Class Summary Page:
<img src="https://github.com/JimLynchCodes/Java-Thoughts/blob/main/JavaCoCo-class-summary.png"/>

<br/>

Java Class Implentation Page:
<img src="https://github.com/JimLynchCodes/Java-Thoughts/blob/main/JavaCoCo-class-source-code.png"/>

<br/>

