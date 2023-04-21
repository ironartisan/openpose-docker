# openpose

A docker build file for CMU openpose-v1.6.0 with Python API support


## Requirements


## Getting started

### cloning the repo.

```
$ git clone https://github.com/ironartisan/openpose-docker.git
```

### build the image using dockerfile

```
$ cd ./openpose-docker
$ sudo docker build -t openpose .

```
### start docker env.
```
nvidia-docker run -tdi  -v ~/data/:/openpose/data/ --net=host -e DISPLAY --runtime=nvidia  --name=openpose openpose:latest

```

### run examples
```
docker exec -it <images> /bin/bash
cd /openpose/examples/tutorial_api_python
python3 01_body_from_image.py
```
