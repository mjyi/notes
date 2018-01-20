# 使用 rbenv 管理 Ruby 版本

在 macOS 下使用 [rbenv][rbenv] 管理 Ruby 版本。


## 安装

1. 推荐合适 homebrew 安装
```bash
brew install rbenv
```

2. 运行`rbenv init` 命令，并按照说明进行设置。如在`zsh` 中
```bash
# Load rbenv automatically by appending
# the following to ~/.zshrc:
eval "$(rbenv init -)"
```

3. 重新打开一个 Terminal 窗口，使更改生效。


## 使用

### 安装 ruby

```bash
rbenv install --list  # 列出所有 ruby 版本
rbenv install 1.9.3-p392     # 安装 1.9.3-p392
rbenv install jruby-1.7.3    # 安装 jruby-1.7.3
```

### 列出版本

```bash
rbenv versions               # 列出安装的版本
rbenv version                # 列出正在使用的版本
```

### 设置版本

```bash
rbenv global 1.9.3-p392      # 默认使用 1.9.3-p392
rbenv shell 1.9.3-p392       # 当前的 shell 使用 1.9.3-p392, 会设置一个 `RBENV_VERSION` 环境变量
rbenv local jruby-1.7.3      # 当前目录使用 jruby-1.7.3, 会生成一个 `.rbenv-version` 文件

rbenv shell --unset          # 取消本地版本
rbenv local --unset          # 取消当前shell版本
```

### 其它

```bash
rbenv rehash                 # 每当切换 ruby 版本和执行 bundle install 之后必须执行这个命令
rbenv which irb              # 列出 irb 这个命令的完整路径
rbenv whence irb             # 列出包含 irb 这个命令的版本
```

## 参考资料

- [rbenv][rbenv]


[rbenv]: https://github.com/sstephenson/rbenv

