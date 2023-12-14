## Coding-simple_2023

# welcome `Anonymous`


# html-image-docker-compose

## This is just a sample project to run docker-compose with a simple html file.

Here are three files
- Dockerfile
- Docker-compose.yaml
- index.html
- nginx.conf


## For docker build

`docker build -t htmltesting .`

`docker run --rm -d -p 5000:80 --name myweblocal htmltesting`

## For running Docker-compose

`docker-compose up -d`

`docker-compose ps`

`docker-compose logs`

You can change index.html for showing different message.

You can run this 



# K8s Config Deployment

`kubectl create configmap nginx-index-html-configmap --from-file=index.html -o yaml --dry-run`

`kubectl deployment index.html -o yaml --dry-run`

`kubectl apply -f nginx.yaml`

`kubectl apply -f nginx-services.yaml`

`kubectl apply -f indexhtml-configmap.yaml`

## copyright2023_devtolearn

> **Note** if you having any issues running docker then run run with sudo as super user priviledges 

