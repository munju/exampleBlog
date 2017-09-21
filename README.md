# Wordpress Docker Example
This example describes the process needed to set up a wordpress blog using docker locally.

## Running it locally
If you only want to deploy your wordpress blog locally, you need a system installed with docker and docker-compose.
Here is a link to help you do that: https://docs.docker.com/engine/installation/

Clone this git repository, move into the directory with the `docker-compose.yml` file and execute the following command:
```bash
docker-compose up -d
```
To shutdown the containers use the following command:
```bash
docker-compose down
```

This wordpress example has already been setup with an admin user.
* username: admin
* password: admin
* email: admin@jmwordpress.com

If a you want to have a clean install just delete the content of the db_data directory.

## Scaling it
To scale this type of application you need to use an application like Docker Swarm or Kubernetes. Those applications allow you to automate deployment, scaling, and management of containerized applications. You will still have to consider the db container needs to be persistent and is not stateless.
