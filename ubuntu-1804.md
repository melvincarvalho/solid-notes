Testing setup on ubuntu 18.04

Provider scaleway

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



