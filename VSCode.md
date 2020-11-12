# Visual Studio Code

Visual Studio Code is one of the famous IDE that is getting increasing attention recently, but downloading it in China needs some trick.

## Download Installer

When downloading the installer from the website `https://code.visualstudio.com/`, the speed is about 0kB - 20kB, which is too slow for a ~70MB package.

What we need to do is replace the website in the url, for example, from:

```url
https://az764295.vo.msecnd.net/stable/e5a624b788d92b8d34d1392e4c4d9789406efe8f/code_1.51.1-1605051630_amd64.deb
```

to:

```url
https://vscode.cdn.azure.cn/stable/e5a624b788d92b8d34d1392e4c4d9789406efe8f/code_1.51.1-1605051630_amd64.deb
```

i.e., replace it into `vscode.cdn.azure.cn`.

## Disable the Source

If you don't know how to disable a source, refer to [Ubuntu](Ubuntu.md).

Disable the source `http://packages.microsoft.com/repos/vscode stable main` in `Other Software` tab in the `Software & Updates` app.

## Reference

- [Speedup the Download of VSCode in China](https://zhuanlan.zhihu.com/p/112215618)