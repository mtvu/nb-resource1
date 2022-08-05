# Setup the docker environment

Notes: Working code - mapping 8080 to local 8082
Point the code folder to work directory 
docker  run -d --name code-server -p 127.0.0.1:8082:8080 \
  -v "/home/abeo/docker/code-server1/.config:/home/coder/.config" \
  -v "/home/abeo/work:/home/coder/project" \
  -u "$(id -u):$(id -g)" \
  -e "DOCKER_USER=$USER" \
  codercom/code-server:latest

# Install conda
curl  https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh 


https://github.com/nowke/realtime-dashboard-demo/
https://dev.to/nowke/building-real-time-dashboard-using-react-graphql-subscriptions-and-redis-pubsub-2gip
