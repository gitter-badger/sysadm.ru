---
layout: page
title: Installing Docker on CentOS
permalink: /docker/basics/installing-docker-on-centos/
---


## 04 Installing and Updating Docker

04 03 Installing Docker on CentOS

У меня сейчас нет под рукой машины с centos. Поэтому только команды:

    # yum install -y docker
    # systemctl status docker.service

    # systemctl start docker.service
    # docker -v
    # docker version
    # docker info