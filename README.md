```
1. docker-compose up -d
2. docker ps
3. docker exec -it mongo1 mongo
4. config = {
    _id: "rp0",
    members: [
      { _id: 0, host: "mongo1:27017" },
      { _id: 1, host: "mongo2:27017" },
      { _id: 2, host: "mongo3:27017" },
    ],
  }
5. rs.initiate(config)
6. rs.conf()  
7. exit
8. connect mongodb form  mongo-url = "mongodb://mongo1:27017,mongo2:27017,mongo3:27017/movie?replicaSet=rp0"
9. create databse
10. create collection
11. insert data into collection
12. get all indexs curl -X GET http://localhost:9200/_cat/indices?v
13. get a index curl -X GET http://localhost:9200/movie/_search?
```