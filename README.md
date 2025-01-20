### Steps to get app running

1. sudo docker start <container-ID>
2. SKIP_DOCKER=true ./scripts/init_db.sh

### Example of how to use database with Docker in terminal

1. docker exec -it <container-ID> psql -U postgres
