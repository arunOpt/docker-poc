# Docker
docker cli (client)=> rest api=> docker daemon

# docker commands
docker run image-name
       |command => run => create a container from img and execute command on it
                => images => list all local image
                => tag => tag an image
                => push => download image from a repository
                => rmi => delete a local image

# Docker Architecture
docker daemon=> bg service to manage image
docker client=> ui to docker
docker image => read only,  instructions to create container
docker container => contain all things required to run

google kubernetes/swarm => manages a lot of containers 

https://get.docker.com/ => to install docker

# 1. download the script
#
#   $ curl -fsSL https://get.docker.com -o install-docker.sh
#
<!-- # 2. verify the script's content
#
#   $ cat install-docker.sh
#
# 3. run the script with --dry-run to verify the steps it executes
#
#   $ sh install-docker.sh --dry-run
#
# 4. run the script either as root, or using sudo to perform the installation.
# -->
#   $ sudo sh install-docker.sh

# Run Docker
sysytemctl start docker

# run hello world container
docker run hello-world

ps -ef => list process
ps -ef |grep dock => process contains dock
ps -A |grep dockerd => all process contains dockerd
ps -A |grep containerd => all process contains containerd

docker ps -a (or) docker container ls