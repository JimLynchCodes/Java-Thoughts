
# PITest Mutation Testing

Mutation testing shows _where you are missing assertions in your unit tests!_

<br/>

## Installing PITest in a gradle java project:

<br/>

Add the `gradle-pitest-plugin` to the plugins configuration in your build.gradle file:

```groovy
plugins {
    id 'info.solidsoft.pitest' version '1.9.0'
}
```

<br/>

Then call Gradle with pitest task:
```bash
gradle pitest
```

<br/>

After the measurements a report created by PIT should be placed in the `/build/reports/pitest` directory.

<br/>

---
