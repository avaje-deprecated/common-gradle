# common-gradle
Common gradle build configuration such as releasing to OSS Sonatype, Runnable War/Jar etc


## steps

### 1. git clone
git clone this repo

### 2. edit gradle.properties
Edit your ~/.gradle/gradle.properties file adding:

```properties
gradle_common=<local path to where this repo is cloned>
```

### 3. apply from
Now you can use `apply from` to incorporate the build scripts

e.g. 
```groovy
apply from: "${gradle_common}/oss.gradle"
```
