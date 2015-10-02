---
layout: page
title: Инсталляция Docker в Ubuntu
permalink: /linux/virtual/docker/basics/installing-docker-on-ubuntu/
---


**Вариант 1: устанавливаем docker из репо ubuntu. (не рекомендую)**

    $ sudo su

    # apt-get update
    # apt-get install -y docker.io
    # service docker.io status

    $ docker -v


**Вариант 2: устанавливаем docker из репо docker. (рекоменую)**

    # wget -qO- https://get.docker.com/gpg | apt-key add -
    # echo "deb http://get.docker.com/ubuntu docker main" >> /etc/apt/sources.list.d/docker.list

    # apt-get update
    # apt-get install -y lxc-docker

    # docker -v


**Предоставить пользователю права для работы с docker**

    $ sudo gpasswd -a <username> docker

в группе docker должен появиться этот пользователь  

    $ cat /etc/group
        docker:x:126:username

перелогиниваемся  

    $logout