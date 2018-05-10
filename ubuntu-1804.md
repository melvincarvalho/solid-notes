Testing setup on ubuntu 18.04

### 1. Instance prep {#1-instance-prep�}

**Select A Server**

Scaleway offers a number of servers. At time of writing it is possible to run a server with unmetered bandwidth, 50 GB of storage and running Ubuntu 18.04 for 3.99 EUR per month. This is the target used in this guide.

**Log in to the machine**

To log into a scaleway server locate the IP addres and ssh to root@ip-address. This will log you in as root.

Install sudo



**Create a User**

It is not desirable to run as root, so it is possible to add a user, ubuntu is selected here.

```
useradd -m ubuntu
sudo usermod -a -G sudo ubuntu
passwd ubuntu
```

You will also want to copy the ssh key into the .ssh directory to allow login via ubuntu@ip-address

```
mkdir /home/ubuntu/.ssh
cp -rp .ssh/* /home/ubuntu/.ssh
chown ubuntu:ubuntu /home/ubuntu/.ssh/*
```

```
chsh -s /bin/bash ubuntu
```



