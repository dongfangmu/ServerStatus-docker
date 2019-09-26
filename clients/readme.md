```
apt-get update \
  &&  apt-get install python-dev  \
     build-essential libssl-dev libffi-dev \
     libxml2-dev libxslt1-dev zlib1g-dev \
     python-pip gawk vnstat \
  && apt-get install -y python python-pip gawk vnstat \
  && pip install psutil \
  && wget https://github.com/drice82/ServerStatus-docker/raw/master/clients/client-psutil.py \
  && nano client-psutil.py
```
###
systemctl start rc-local
chmod +x rc.local
rc.local
```
#!/bin/sh -e
nohup python /root/client-psutil.py &> /dev/null &
exit 0
```
