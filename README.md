# 1key-zmk-config

## usage

build example using [zmk-docker-containter]()

```
cd ~/Downloads
git clone git@github.com:hidsh/1key-zmk-config.git

docker run -it -d -v /mnt/d/_downloads/1key-zmk-config:/root/1key zmk-x86-64 /bin/bash
docker attach <container id>
cd ~/1key 
west build -s ~/zmk/app -p -b seeeduino_xiao -- -DSHIELD=1key -DZMK_CONFIG=$PWD/config
```
