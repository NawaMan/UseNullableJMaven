# UseNullableJMaven
Example of how to use NullableJ in a Maven project.

It basically boils down to adding dssb maven repository (hosted by github).

```xml
	<repositories>
		<repository>
			<id>DssbUtils-mvn-repo</id>
			<url>https://raw.githubusercontent.com/nawaman/nawaman-maven-repository/master/</url>
			<snapshots>
				<enabled>true</enabled>
				<updatePolicy>always</updatePolicy>
			</snapshots>
		</repository>
	</repositories>

	<dependencies>
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
	</dependencies>
```
See the full code here: (pom.xml)[https://github.com/NawaMan/UseNullableJMaven/blob/master/pom.xml]
