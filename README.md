## Requires   
* docker
# Usage   
```bash
#build the docker image
./build.sh
#launch the container
./launch_container.sh
# this makes a new container
```   

### Relevant commands
If you followed the docker setup and added the docker user, you don't need sudo to run these commands.
```bash
# show running containers
sudo docker ps
# show all containers including old stopped containers
sudo docker ps -a
```
```bash
CONTAINER ID   IMAGE     COMMAND       CREATED        STATUS        PORTS     NAMES
b386db9a6164   troute    "/bin/bash"   17 hours ago   Up 17 hours             quizzical_chebyshev
```
```bash
# to start a stopped container
sudo docker start <container name or id>
sudo docker start quizzical_chebyshev

# to open an interactive shell in the container
sudo docker exec -it <container name or id> bash
sudo docker exec -it quizzical_chebyshev bash
```
