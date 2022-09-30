# 安装anaconda

## 访问官网下载最新的release
[anaconda官网](https://www.anaconda.com/products/distribution#Downloads)

## 执行.sh文件

```bash
./Anaconda3-2022.05-Linux-x86_64.sh
```
安装过程中间遇到的条款一般都填yes

## 重启terminal

重启终端的第一种办法是重启机器

```bash
reboot
```

不想重启电脑可以重新ssh远程连接。或者重新导入环境变量

```bash
source ~/.bashrc
```

# 进入anaconda虚拟环境

```bash
conda deactivate
conda activate your_env_name
```
