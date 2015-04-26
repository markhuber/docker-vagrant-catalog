## docker-vagrant-catalog
Docker container for http://github.com/vube/vagrant-catalog

## Description
This is a docker container based on [tutum/apache-php](https://registry.hub.docker.com/u/tutum/apache-php/) which automatically clones [vube/vagrant-catalog](github.com/vube/vagrant-catalog) and installs all necessary dependencies. 

## Vagrant Box Files
The container assumes the Hashicorp Atlas folder structure and metadata.json file schemas. For more details see this post on [Your own Vagrant Cloud](https://medium.com/@jonursenbach/your-own-vagrant-cloud-f077625c6ac8). You should create this folder structure somewhere and use a volume to mount it in to the container.

## Instructions
To run:
```bash
docker run -d -p 80:80 -v /path/to/files:/var/www/html/files
```

