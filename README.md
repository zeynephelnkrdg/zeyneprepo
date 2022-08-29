# Zeynep Helin Karadağ Minikube

After writing the API code, the command I use to run the API in Docker is:

docker build -t golangwebapi .

I wrote the commands I used to create a path, copy the files on the host to that path, and then run which golang version I was using in the Dockerfile.

To push the image to Dockerhub I created a profile and and I uploaded the image there by entering the username and password of this account in the terminal with docker push command.
After pushing the image I started minikube with minikube start command and I used kubectl create -f kubernetes.yaml to run the yaml file.
In the YAML file, I specified which kubernetes API I used to run the image I created, what kind of object I used, the name and port number of the container I used while running it.

The error I got after the code I wrote to list the running pods:
Unable to connect to the server: net/http: TLS handshake timeout.




