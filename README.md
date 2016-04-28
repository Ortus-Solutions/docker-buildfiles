# Ortus Solutions Docker Build Files

Dockerfiles and configs for Box Products builds and testing


Instructions
------------

The files in this repos may be cloned and used during the build process.  See the `docker-compose` example files for different configurations.  

For installation and multi-engine testing on a local machine you will need to install Docker and Docker Compose.  Then, with the `docker-compose.yml` file in the root of your project, build and spool up the test servers with:

```
docker-machine start default
docker-compose build
docker-compose up -d
```

The `-d` flag used in `up` will start the process as a daemon. `docker-machine ls` will show you the IP address of your docker machines.  To stop the servers simply run `docker-compose stop` from the root of your project.
