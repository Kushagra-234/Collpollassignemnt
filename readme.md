### Note: Docker must be install



###  run the compose file to start sql database and redis-cache service

```
docker-compose up
```

### build image - 

```
./mvnw spring-boot:build-image
```


### run server
```
./mvnw spring-boot:run -Dspring-boot.run.profiles=mysql
```

## Updates for integrating redis-chache- 

### Added Dependencies for redis- 

https://github.com/Kushagra-234/Collpollass/blob/90fffcab0e2c4d7f85db6332cdbfa0b010cdd528/pom.xml#L63-L75

### Added redis Service in compose-file

https://github.com/s-pratyush/spring-project/blob/90fffcab0e2c4d7f85db6332cdbfa0b010cdd528/docker-compose.yml#L25-L31

### Updated cache config file

https://github.com/s-pratyush/spring-project/blob/90fffcab0e2c4d7f85db6332cdbfa0b010cdd528/src/main/java/org/springframework/samples/petclinic/system/CacheConfiguration.java#L1-L72

