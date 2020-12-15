# Nodejs

To use the original source of Node, we need to set the proxy and https-proxy.

## Set proxy and https-proxy

Suppose we have a proxy running at `127.0.0.1:8889`.

```shell
npm config set proxy http://127.0.0.1:8889
npm config set https-proxy http://127.0.0.1:8889
```

## Remove proxy and https-proxy

Suppose we have a proxy running at `127.0.0.1:8889`.

```shell
npm config rm proxy
npm config rm https-proxy
```

## Reference

- [How to configure npm, git and bower for Visual Studio behind a proxy](https://stackoverflow.com/questions/41038067/how-to-configure-npm-git-and-bower-for-visual-studio-behind-a-proxy#:~:text=In%20the%20Visual%20Studio%20developer%20command%20window%2C%20type,type%20this%20command%3A%20npm%20config%20set%20https-proxy%20http%3A%2F%2Fproxyuser%3Aproxypwd%40proxy.server.com%3A8080.)
- [How to clear https proxy setting of NPM?](https://stackoverflow.com/questions/21228995/how-to-clear-https-proxy-setting-of-npm#:~:text=By%20running%20npm%20config%20rm%20proxy%20you%20remove,clean-up%20proxies%20from%20both%20local%20and%20global%20configs%3A)
