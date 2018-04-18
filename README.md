# ppdockerabetterwabuiapps

## What is a container
- Contains everything an application needs
- Applications are isolated from each other
- Easily distributed to other locations
- Uniform management across cloud providers

### Installing Docker on AWS,Google Compute Engine
last flag is name of machine.
```
docker-machine create --driver amazonec2 --amazonec2-region us-west-2 --amazon
ec2-ami ami-0c3abaa6c --amazonec2-ssh-user centos name
```

```
eval $(docker-machine env name)
```


### Managing Containers
```
docker container run -it --name=bb busybox:1.25
```
interactively and sudo tty. leave it by ctrl p q. reattach
```
docker attach bb
```
if
```
exit
```
then
```
docker container start bb
```

### Single-node Networking
#### The bridge network in more detail
