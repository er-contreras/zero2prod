### Steps to get app running

If Docker image has not created yet, try the next.
```docker run -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=password -e POSTGRES_DB=newsletter -p 5432:5432 -d postgres postgres -N 1000```

Then you can follow the next steps!

In case you already have an Docker image try the next.
1. sudo docker start <container-ID>
2. SKIP_DOCKER=true ./scripts/init_db.sh

### Steps to build from Dockerfile
```docker build --tag zero2prod --file Dockerfile .```
docker run -p 8000:8000 zero2prod

### Example of how to use database with Docker in terminal

1. ```docker exec -it <container-ID> psql -U postgres```

### Example of how to make a post request.

1. ```curl -i -X POST -d 'email=thomas_mann@hotmail.com&name=Tom' http://127.0.0.1:8000/subscriptions```
