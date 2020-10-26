# Ubuntu

The latest LTS version of Ubuntu is 20.04. I will take Ubuntu 20.04 as an example, but it should be quite similar to other versions.

To change the source of Ubuntu 20.04, we can change it manually or change the source using graphical interface.

## Graphical Interface

> Note: since it's easy to choose from the drop-down menu, this way is preferred.

1. Go to **Software & Updates**
2. Under **Ubuntu Software** tab, change the **Download from** to **http://mirrors.aliyun.com/ubuntu**
3. Update the cache: `sudo apt update`

## Manually

> Note: this is not recommended.

1. Make a backup of the source list file: `copy /etc/apt/sources.list /etc/apt/sources.list.backup`
2. Open the source list file: `vim /etc/apt/sources.list`
3. Change the default address `http://archive.ubuntu.com` into `http://mirrors.aliyun.com`
4. Update the cache: `sudo apt update`

## Reference

1. [Aliyun's Mirror](https://developer.aliyun.com/mirror/ubuntu?spm=a2c6h.13651102.0.0.3e221b117iQ1ae)