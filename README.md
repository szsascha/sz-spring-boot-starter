# SZ Spring Boot Starter

I often start my own Spring Boot projects with the same setup. I would like to standardize this in the future. So for future projects I will use this starter.

# Modules

## service

The sz-spring-boot-starter-service is used to have a basic setup for services. This module contains primarly the following libraries:

1. spring-boot-starter-web
2. spring-boot-starter-sleuth
3. spring-boot-starter-test
4. lombok (used to save lines of code by annotations)
5. log4j
6. junit
7. mockito

## persistence

sz-spring-boot-starter-persistence gives you a basic setup for persistence, including the following libraries:

1. spring-boot-starter-data-jpa
2. h2
3. mapstruct (used to map dto's to persistence models)
4. hibernate

# Setup

The following steps are required to setup your project with the sz-spring-boot-starter in your maven pom.xml.

## Add jitpack repository

```xml
<repositories>
    <repository>
        <id>jitpack.io</id>
        <url>https://jitpack.io</url>
    </repository>
</repositories>
```

## Add sz-spring-boot-starter-parent

```xml
<parent>
    <groupId>com.github.szsascha.sz-spring-boot-starter</groupId>
    <artifactId>sz-spring-boot-starter-parent</artifactId>
    <version>1.0.0</version>
</parent>
```

# Usage

Now you can add your sz-spring-boot-starters as depdendency.

```xml
<dependencies>
    <dependency>
        <groupId>com.github.szsascha.sz-spring-boot-starter</groupId>
        <artifactId>sz-spring-boot-starter-service</artifactId>
        <version>1.0.0</version>
    </dependency>
</dependencies>
```

After that you're able to use all the dependencies and functionality from the used starters.