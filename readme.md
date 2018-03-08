## Manual

Start mongodb container
```
docker container run -d --name mong1 -p 27017:27017 mongo
```

Build app image
```
docker image build -t toystore .

```

Lunch application from app image
```
docker container run -link mongo1:mongo -p 8080:8080 toystore
```

## Ref

- [MongoDB with Spring Data](https://spring.io/guides/gs/accessing-data-mongodb/)
- [Problem with using mix JPA and Mongodb driver](https://stackoverflow.com/questions/38474164/how-to-connect-to-mongodb-in-springboot)