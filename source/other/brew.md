# Homebrew

`Homebrew` 作为 Mac 下的软件包管理工具，非常好用。

### 安装 & 卸载

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
 
*卸载*
```sh
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/uninstall)"
```

### 安装一个包
```sh
brew install wget
```

### 更新本地软件

1. 更新 Homebrew. 
```sh
brew update
```

2. 查找可更新的软件包
```
brew outdated
```

3. 更新所有过时软件包
```
brew upgrade
```
或者指定更新
```
brew upgrade <formula>
```

### 禁止某些 formulae 更新
```sh
brew pin <formula>

brew unpin <formula>
```

### 卸载旧版本的软件包

```sh
# specific one
brew cleanup <formula>

# clean up everything at once
brew cleanup

# to see what would be cleaned up
brew cleanup -n
```
