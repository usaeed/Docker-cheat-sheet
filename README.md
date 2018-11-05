# Docker-cheat-sheet
# Some useful commands for docker developers and administrators

# Complete wipe out of docker containers and images from a PC.

# Stop all running containers. 
docker stop $(docker ps -aq)

# Remove all containers. 
docker rm $(docker ps -aq)

# Remove all images.
docker rmi $(docker images -q)

# Remove the image even if it is used by containers or having multiple tags
docker rmi -f $(docker images -q)
