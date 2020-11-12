# Sogou Pinyin Input Method

Usually working in China requires that we use Chinese input method. Sogou Pinyin input method is a good choice, but it has some dependency issue on Ubuntu 20.04.

## Download Package

Download the package from the website: [https://pinyin.sogou.com/linux/](https://pinyin.sogou.com/linux/).

## Try Installing it

Run:

```shell
sudo dpkg -i <the package name>
```

It will tell us that it has met some dependency issue.

## Install Dependencies

Run:

```shell
sudo apt install -f
```

This command will install any broken dependencies. Because in the second step, `apt` has found some broken dependencies, this step will help us fix them.

## Re-install Sogou Pinyin

Run:

```shell
sudo dpkg -i <the package name>
```

## Remove ibus (Do it if necessary)

Run:

```shell
sudo apt purge ibus 
```

Then run:

```shell
sudo apt autoremove ibus*
```

When I ran the second command, I didn't succeed, so I change it to:

```shell
sudo apt autoremove ibus
```

## Reference

- [Install Sogou Pinyin on Ubuntu 20.04](https://blog.csdn.net/Mr_FenKuan/article/details/107215026?utm_medium=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.channel_param&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.channel_param)