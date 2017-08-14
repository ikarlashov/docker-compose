========= DETAILS =========

Nginx is built from Dockerfile.

Data from containers is attached to host system.

nginx:

/data/nginx

postgresql:

/data/postgresql

artifactory:

/data/artifactory

PostgreSQL listens on localhost interface. 

Artifactory version could be set by environment variable. If variable isn't set or empty, default Artifactory version is set to 5.4.5.

========= RUN COMMAND =========

$ ARTI_VERSION=5.4.5 docker-compose up -d


========= STOP COMMAND =========

docker-compose stop

========= STOP & REMOVE CONTAINERS ==========

docker-compose stop && docker-compose rm -v
