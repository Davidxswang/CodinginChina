# Docker

The sources of Docker should be set to China sources in China, reset out of China.

## Windows

Go to Settings of Docker, then go to Docker Engine tab. Set the `registry-mirrors` as follows:

```json
"registry-mirrors": [
    "https://registry.docker-cn.com",
    "http://hub-mirror.c.163.com",
    "https://3laho3y3.mirror.aliyuncs.com",
    "http://f1361db2.m.daocloud.io",
    "https://mirror.ccs.tencentyun.com"
  ]
```

## Linux

Add a file `/etc/docker/daemon.json`, and add the following content into the file:

```json
{
"registry-mirrors": [
    "https://registry.docker-cn.com",
    "http://hub-mirror.c.163.com",
    "https://3laho3y3.mirror.aliyuncs.com",
    "http://f1361db2.m.daocloud.io",
    "https://mirror.ccs.tencentyun.com"
  ]
}
```

## Reference

- [Settings for Docker on Windows in China](https://blog.csdn.net/qq_35976271/article/details/91362620)
- [Docker Speedup in China](https://www.cnblogs.com/nhdlb/p/12567154.html)