# Oh My Zsh

[Oh-My-Zsh](https://ohmyz.sh/) is a delightful and open source framework or Zsh.

Before installing oh-my-zsh, zsh is needed to be installed. Just run:

```shell
sudo apt-get install zsh
chsh -s $(which zsh) # set the default shell to be zsh
```

To install it in China, follow the following links.

- [oh-my-zsh国内镜像安装](https://igmainc.github.io/2021/04/17/oh-my-zsh%E5%9B%BD%E5%86%85%E9%95%9C%E5%83%8F%E5%AE%89%E8%A3%85.html)

After install Oh-My-Zsh, we need to install two plugins `zsh-autosuggestions` and `zsh-syntax-highlighting`, follow the [link](https://gist.github.com/dogrocker/1efb8fd9427779c827058f873b94df95) to install them.

When using it, if some words are repeated when auto-completing the command, we might need to set the `locales`, e.g., if on Ubuntu 18.04, run the following command to reset the languages.

```shell
sudo apt-get install locales
sudo dpkg-reconfigure locales
# choose en_US.UTF-8
```

In the `.zshrc`  file, set the variables:

```shell
export LANG=en_US.UTF-8
export LC_ALL=en_US.UTF-8
```

Then run `source .zshrc` will solve the problem.

## References

- [Oh-My-Zsh](https://ohmyz.sh/)
- [oh-my-zsh国内镜像安装](https://igmainc.github.io/2021/04/17/oh-my-zsh%E5%9B%BD%E5%86%85%E9%95%9C%E5%83%8F%E5%AE%89%E8%A3%85.html)
- [Oh my zsh with autosuggestions & syntax-highlighting.md](https://gist.github.com/dogrocker/1efb8fd9427779c827058f873b94df95)
- [Command duplicated on tab completion with oh-my-zsh and Hyper #300](https://github.com/sindresorhus/pure/issues/300)
- [Mac终端使用oh-my-zsh中文乱码](https://blog.csdn.net/weixin_44649870/article/details/104423570)