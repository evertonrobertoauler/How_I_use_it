# Docker on Fedora

Instalation

      sudo yum -y install docker-io
      sudo systemctl start docker
      sudo systemctl enable docker
      
Run first container with ubuntu image

      sudo docker run -i -t ubuntu /bin/bash
      
Save changes as new image

      sudo docker commit -m="some message" -a="Your name" containerId imageName
      sudo docker commit -m="some message" -a="Everton" 1493d35c9315 test/postgres
      
List containers running

      sudo docker ps
      
Delete saved image

      sudo docker rmi -f imageId
      sudo docker rmi -f db0fe432f398
      
List images

      sudo docker images
      
Run image

      sudo docker run -t -i test/postgres /bin/bash
