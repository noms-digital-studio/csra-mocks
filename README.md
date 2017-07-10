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