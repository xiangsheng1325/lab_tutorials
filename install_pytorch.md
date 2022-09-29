# 安装PyTorch
三步安装好pytorch

## 第一步
安装anaconda，把anaconda官网的.sh文件下载下来之后直接输入下面的代码安装：

```bash
./Anaconda.sh
```

各种条款你都同意，就安装好了，然后重启terminal以更新环境变量，不想重启的话就输入：
```bash
source ~/.bashrc
```

## 第二步
安装python37/38/39，输入下面几行代码就能创建新的python虚拟环境

```bash
conda create -n DeepLearn python=3.7
conda activate DeepLearn
```

如果你需要用gpu来跑pytorch，可以用下面这行代码来创建虚拟环境

```bash
conda create -n DeepLearn -c nvidia python=3.7 cudatoolkit=11.6
```

## 第三步
安装pytorch，输入下面几行代码即可在你的虚拟环境下安装你想要的pytorch

```bash
conda deactivate
conda activate DeepLearn
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu116
```

你也可以选择不用pip安装，直接用conda安装：

```bash
conda install pytorch torchvision torchaudio cudatoolkit=11.6 -c pytorch -c conda-forge
```
