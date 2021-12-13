
## package
```bash
mvn clean package -DskipTests=true
```

## deploy nexus
```bash
mvn clean deploy -am -DskipTests
```
### premise
add in the maven installation directory setting.xml
```
     <server>
	  <id>wieof-nexus-releases</id>
	  <username>admin</username>
	  <password>pssword</password>
	 </server>
	 <server>
	  <id>wieof-nexus-snapshots</id>
	  <username>admin</username>
	  <password>password</password>
	 </server>

```

## run test
```bash
java -jar target/jb-hello-world-maven-0.1.0.jar
# or
java -cp target/jb-hello-world-maven-0.1.0.jar hello.HelloWorld
```
