# Exercices Docker Devops

## Maylis LE BORGNE - EPSI B3


## Prise en main
    docker pull ubuntu:latest
    docker build . -t ubuntu
    docker images
    docker run ubuntu
    docker run -it ubuntu /bin/bash
    docker ps

    docker build --pull --rm -f "Dockerfile_prise" -t devopsdocker:latest "."

## Jenkins
### Après l'écriture du fichier Dockerfile

docker build -t jenkins-docker .

```
docker run --name jenkins-master -d -p 8080:8080 -p 50000:50000 -v /var/jenkins_home jenkins/jenkins:lts
```

# je m'identifie avec le initialAdminPassword puis je créer un utilisateur
# sur l'interface de créer un projet puis je lance un build


# Nginx
docker pull nginx
docker run --name docker-nginx -p 40:40 nginx