```
apt-get update \
  && apt-get install -y python python-pip gawk vnstat \
  && pip install psutil \
  && wget https://github.com/drice82/ServerStatus-docker/raw/master/clients/client-psutil.py \
  && nano client-psutil.py
```
