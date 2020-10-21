# Homebrew

We need to use the sources in China to speed up the Homebrew on Mac.

There are three sources we need to change:

1. brew.git
2. homebrew-core.git
3. homebrew-bottles

We will choose Alibaba as the sources in China.

## When in China

### brew.git

```shell
cd "$(brew --repo)"
git remote set-url origin https://mirrors.aliyun.com/homebrew/brew.git
```

### homebrew-core.git

```shell
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://mirrors.aliyun.com/homebrew/homebrew-core.git
```

### homebrew-bottles

This depends on the shell we are using, either `zsh` or `bash`.

#### In zsh

```shell
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.aliyun.com/homebrew/homebrew-bottles' >> ~/.zshrc
source ~/.zshrc
```

#### In bash

```shell
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.aliyun.com/homebrew/homebrew-bottles' >> ~/.bash_profile
source ~/.bash_profile
```

## When not in China

### brew.git

```shell
cd "$(brew --repo)"
git remote set-url origin https://github.com/Homebrew/brew.git
```

### homebrew-core.git

```shell
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://github.com/Homebrew/homebrew-core.git
```

### homebrew-bottles

This depends on the shell we are using, either `zsh` or `bash`.


#### In zsh

1. Open `~/.zshrc`
2. Delete the line we inserted `export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.aliyun.com/homebrew/homebrew-bottles`
3. Apply the changes, `source ~/.zshrc`

#### In bash

1. Open `~/.bash_profile`
2. Delete the line we inserted `export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.aliyun.com/homebrew/homebrew-bottles`
3. Apply the changes, `source ~/.bash_profile`

## Reference

1. [How to Speed up Homebrew in Mac](https://www.jianshu.com/p/397860ff2a0e)