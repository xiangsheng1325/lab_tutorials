# 为什么要注册虚拟环境？

我们在服务器安装了新的虚拟环境后，在jupyterlab里暂时还找不到新建的kernel。
因此我们需要在jupyterlab上为虚拟环境注册一个新kernel，注册了就能在jupyterlab用新环境跑代码了。

# 在jupyterlab上注册虚拟环境

注册之前记得先[安装anaconda](https://github.com/xiangsheng1325/lab_tutorials/blob/main/install_anaconda.md)

## 先进入你的虚拟环境

```bash
conda activate your_env
```

## 再安装依赖库

```bash
pip install ipykernel
```

## 最后一行代码注册你的虚拟环境

```bash
python -m ipykernel install --name your_env_name --user
```

## 刷新一下网页

刷新网页后就能看见jupyterlab上注册了新的虚拟环境，可以直接把kernel更改为你自定义的environment。
