### Steps to get app running

1. sudo docker start <container-ID>
2. SKIP_DOCKER=true ./scripts/init_db.sh

### Example of how to use database with Docker in terminal

1. docker exec -it <container-ID> psql -U postgres

### Example of how to make a post request.

1. ```curl -i -X POST -d 'email=thomas_mann@hotmail.com&name=Tom' http://127.0.0.1:8000/subscriptions```
