# getting started

### Command

### Make container

* for small machine
```bash
nvidia-docker run -it --shm-size=4gb --cpus=4 -e NVIDIA_VISIBLE_DEVICES=0,1 -v $(pwd):/workspace pytorch/pytorch:1.6.0-cuda10.1-cudnn7-devel /bin/bash
```

* for giant machine

```bash
nvidia-docker run -it --shm-size=32gb --cpus=32 -e NVIDIA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 -v $(pwd):/workspace pytorch/pytorch:1.6.0-cuda10.1-cudnn7-devel /bin/bash
```

### install

```bash
pip install tensorboard
```
