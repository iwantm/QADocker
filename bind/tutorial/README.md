for volume: docker run -d -v project-db:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=pass -e MYSQL_DATABASE=event --network flask-network --name new-sql mysql:5.7 
bind mount: docker run -d --network flask-network --mount type=bind,source=$(pwd)/CreateTable.sql,dst=/docker-entrypoint-initdb.d/ -e MYSQL_ROOT_PASSWORD=pass  -e MYSQL_DATABASE=flask-db --name mysql mysql:5.7
