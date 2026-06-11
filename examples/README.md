# Learn Docker with examples

INSTALL DOCKER

A very detailed instructions to install Docker are provide in the below link

https://docs.docker.com/get-docker/

For Demo, 

You can create an Ubuntu EC2 Instance on AWS and switch to root user and run the below commands to install docker.

```
apt update
apt install docker.io -y
```

A easy way to verify your Docker installation is by running the below command

```
docker run hello-world
```
Output should look like:

```
....
....
Hello from Docker!
This message shows that your installation appears to be working correctly.
...
...
```
### Clone this repository and move to example folder

```
git clone https://github.com/nikhilsadawarti/Docker-Projects
cd  examples/python-web-app
```
Build Docker Image
```
docker build .
```
Verify Docker Image is created
```
docker images
```
Run Docker Container
```
docker run -it <IMAGE ID>
```
Port mapping on container 
```
docker run -p 8000:8000 -it <IMAGE ID>
```
Open browser and access http://<<PUBLICIP>>:8000/demo/ with PUBLIC IP
