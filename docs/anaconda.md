为了方便多个科研项目同时开发，不导致包之间的冲突，我们使用Anaconda进行环境的管理。

可以说，Anaconda是深度学习的研究人员必备的工具之一。

我们在机器上预装了Anaconda3, 可以使用anaconda方便的管理环境的package依赖。
使用anaconda安装包的好处在于它能自动的帮你解决安装package过程中的依赖，会把附属包也一并装上。
如果下载速度太慢，请设置conda的源为清华源。可以通过修改用户目录下的 .condarc 文件。
```shell
channels:
  - defaults
show_channel_urls: true
channel_alias: https://mirrors.tuna.tsinghua.edu.cn/anaconda
default_channels:
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/r
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/pro
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/msys2
custom_channels:
  conda-forge: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  msys2: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  bioconda: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  menpo: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  pytorch: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  simpleitk: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
```
即可添加 Anaconda Python 免费仓库。

## 常见的conda命令

### 查看已有环境
```shell
conda info --envs
```

### 创建新的环境
```shell
conda create -n your_env_name
```

### 切换到新的环境
```shell
conda activate your_env_name
```

### 安装package
```shell
conda install package_name
```
或者使用pip
```shell
pip install package_name
```







