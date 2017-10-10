# Installing Dependencies
You will need to have JDK (Java SE Development Kit) installed on your system
[http://www.oracle.com/technetwork/java/javase/downloads/index.html](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
or
```
brew cask install java
```

You will also need Gradle installed on your system
```
brew install gradle
```

# To build and run the fat JAR
```
./gradlew clean shadowJar
java -jar build/libs/csra-mocks-all.jar --root-dir src/main/resources --port 9090
```

# To run via Gradle
```
./gradlew clean run
```

# To view default mappings
```
curl http://localhost:9090/__admin/
```

# Example defaults
```
curl -H "API-Key:valid-subscription-key" http://localhost:9090/offender/J1234LO/viper
curl -H "API-Key:valid-subscription-key" http://localhost:9090/offender/NOTFOUND/viper
```