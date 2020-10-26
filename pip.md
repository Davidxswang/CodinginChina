# pip

We need to change the pip source to speed up the process when using pip to install the software, e.g., to use Aliyun's mirror.

## Ubuntu

1. Create a pip configuration file in $HOME directory: `vim ~/.pip/pip.conf`
2. Change the content of the file as follows.

```conf
[global]
index-url = https://mirrors.aliyun.com/pypi/simple/

[install]
trusted-host=mirrors.aliyun.com
```

## Mac

Same with Ubuntu

## Windows

1. Create a pip configuration file in user's directory, e.g., `C:\Users\david\pip\pip.ini`
2. Change the content of the file as above.

## Reference

1. [Faron's blog](https://www.cnblogs.com/printN/p/7382814.html)
2. [Aliyun's mirror](https://developer.aliyun.com/mirror/pypi?spm=a2c6h.13651102.0.0.3e221b117iQ1ae)