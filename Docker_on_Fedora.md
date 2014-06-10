# Docker on Fedora

Instalation

      sudo yum -y install docker-io
      sudo systemctl start docker
      sudo systemctl enable docker
      
Run first container with ubuntu image

      sudo docker run -i -t ubuntu /bin/bash

List containers running

      sudo docker ps
      
List images available

      sudo docker images
      

Save changes as new image

      sudo docker commit -m="some message" -a="Your name" containerId imageName
      sudo docker commit -m="some message" -a="Everton" 1493d35c9315 test/postgres
      
      
Delete saved image

      sudo docker rmi -f imageId
      sudo docker rmi -f db0fe432f398
      
Run image

      sudo docker run -t -i test/postgres /bin/bash
