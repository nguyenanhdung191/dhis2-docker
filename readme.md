# How to use:

## Init containers

1. Open terminal/cmd in root folder, run `docker-compose build`

## For first time running

1. Copy dhis2 WAR file to ./dhis2 and name it `dhis2.war`
2. Create folder `data` and `backup` in ./postgresql
3. Put database dump in ./postgresql/backup (.sql or sql.gz) (if using fresh database, skip this step)
4. Open terminal/cmd in root folder, run `docker-compose up postgresql`, and wait for the container to finish restoring database
5. Stop postgresql container (Ctrl - C)
6. Open terminal/cmd in root folder, run `docker-compose up`
7. Dhis2 instance is ready on localhost:80

## For after first time running

1. Open terminal/cmd in root folder, run `docker-compose up`
2. Dhis2 instance is ready on localhost:80
