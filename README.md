docker container run -d \
-p 3001:3001 \
--env DB_USER=root \
--env DB_NAME=newsfeed_db \
--env DB_PASSWORD=123456789! \
--env DB_HOST=172.17.0.2 \
--link mysql-db:db \
--name=node-app newsfeed-app