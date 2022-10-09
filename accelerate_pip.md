# 用镜像加速pip安装

## 执行如下代码

```bash
mkdir ~/.pip
vim ~/.pip/pip.conf
```

## 在pip.conf文件当中输入如下内容

```
[global]
index-url = https://mirrors.aliyun.com/pypi/simple/
```

保存文件后pip下载就会优先搜索index-url的镜像地址，一般来说加速效果显著。

如果觉得阿里云镜像慢，可以搜一下网上的其他pypi镜像，例如清华镜像和豆瓣。
