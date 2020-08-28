# simple-web
This repository for Infrastructure Engineer - eFishery Skill Test

## Getting Started

You need to install Docker, kubectl, and Minikube. More detail you can check on these documentation 

```

https://docs.docker.com/engine/install/
https://kubernetes.io/docs/tasks/tools/install-kubectl/
https://kubernetes.io/docs/tasks/tools/install-minikube/

```

## Running the tests

### Build Docker Image
You can build and push this image into Docker Hub repository using this command

```

$ docker build -t <docker-hub-id>/simple-web:tagname
$ docker push <docker-hub-id>/simple-web:tagname


```

### Deploy the app into minikube
You can deploy and test this app running well using this command

```

$ minikube start
$ kubectl apply -f k8s-manifest/
$ kubectl get pods
$ kubectl port-forward <pod-name> 80:80
    
```

To access the app, you can use this command 

```

$ curl localhost:80 

```

or type it into browser

```

http://localhost:80

```

## Built With

* [Kubernetes] (http://www.kubernetes.io) 
* [Docker] (https://docs.docker.com/get-docker/)  

## Authors

* **Hakim Rizki Pratama** - *DevOps Engineer* - [hakimrizki](https://github.com/hakimrizki)


