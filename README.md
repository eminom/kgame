https://blog.csdn.net/Accepted_Lam/article/details/103837677


* Add user

```bash
useradd -m xxx
```

useradd -u idxxxx xxx
to make the user share the same id as the host

if the id is not the same, use

```bash
userdel xxx
```

to remove the old one


Some packages are very larage, and may not be recommended to installed into the initiative container
Such as xgboost

Consider install PyTorch, imageio manually


Install libgl1-mesa-dev in order to solve the "import cv2" problem

* Recommended packages

- PyTorch(Cpu version, most probably)
- python3 -m pip install imageio
- python3 -m pip install torchviz
- apt install -y wget
- build graphviz from source and install
- python3 -m pip install tensorboard
- python3 -m pip install gym
- python3 -m pip install pygame
- python3 -m pip install seaborn
* And also

- install kaggle-environments


* Stop and rerun due to new port mapping

```bash
docker stop A
docker commit A imageA #
docker rm A
docker run -d -p 80:80 --name A imageA
```


