# UseNullableJMaven

![alt "Build status"](https://travis-ci.org/NawaMan/UseNullableJMaven.svg?branch=master)

Example of how to use NullableJ in a Maven project.

It basically boils down to adding NawaMan maven repository (hosted by github).

```xml
<repository>
	<id>Nullable-mvn-repo</id>
	<url>https://raw.githubusercontent.com/nawaman/nawaman-maven-repository/master/</url>
	<snapshots>
		<enabled>true</enabled>
		<updatePolicy>always</updatePolicy>
	</snapshots>
</repository>
```

and the required dependencies ...

```xml
<dependency>
	<groupId>nawaman</groupId>
	<artifactId>nullablej</artifactId>
	<version>0.4.0</version>
</dependency>
<dependency>
	<groupId>junit</groupId>
	<artifactId>junit</artifactId>
	<version>4.11</version>
	<scope>test</scope>
</dependency>
```
See the full code here: [pom.xml](https://github.com/NawaMan/UseNullableJMaven/blob/master/pom.xml)

