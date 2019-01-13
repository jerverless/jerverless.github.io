# Developer Guide

## Requirements
- JDK 1.8

## Getting started

Clone the repository in your local directory

```bash
 $ git clone <forked_url>
```

We are using gradle as the build tool.
This command will download and install gradle, then it will build the jar file.

> Windows users may use **.\gradlew** _instead_ of **./gradlew**
> It applies to all bash commands listed below.

```bash
 $ ./gradlew assemble
```

The resulted jar file can be found in `build/libs`

```
 $ java -jar build/libs/jerverless-0.1.0.jar 
```

Or run 

```bash
 $ ./gradlew assembleDist
```

This will create distributions of `jerverless`, you can find them in `build/distributions/`

To install this distribution in a path you desired try out

```bash
 $ ./gradlew installDist
```

By default it will be installed in `build/install/jerverless`

To run the distribution, try

```bash
 $ build/install/bin/jerverless
```
