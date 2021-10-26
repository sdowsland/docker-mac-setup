# docker-mac-setup

## Install Multipass

https://multipass.run/

## Create Multipass VM

```bash
multipass launch ubuntu -n docker-machine -c 2 -m 8G -d 20G
```



## Mount local home directory to vm

```
multipass mount $HOME docker-machine
```

## Log into VM

```
multipass shell docker-machine
```

## Install docker and add ubuntu to group

```
sudo apt-get update
sudo apt-get install docker.io
sudo usermod -aG docker $USER
```

## Add your SSH public key to the VM so you can SSH in

```

```


## Now exit the VM

```
exit
```

