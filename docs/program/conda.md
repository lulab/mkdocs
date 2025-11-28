# Conda/python in Linux

> **Install miniconda (python & pip included) in Linux**
>
> see more in [Recommended Software for Python](https://book.ncrnalab.org/teaching/part-i.-programming-skills/3.python#id-4-recommended-software-for-python)


##  1.miniconda

**(need to repeat it for each user)**

清华镜像网站安装帮助： <https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/>

Miniconda 是一个 Anaconda 的轻量级替代，默认只包含了 python 和 conda，但是可以通过 pip 和 conda 来安装所需要的包。Miniconda 安装包可以到以下链接下载。

<https://mirrors.tuna.tsinghua.edu.cn/anaconda/miniconda/>


```bash
# step 1. download the installation script
wget https://mirrors.tuna.tsinghua.edu.cn/anaconda/miniconda/Miniconda3-latest-Linux-x86_64.sh

# step 2. install
bash Miniconda3-latest-Linux-x86_64.sh
```

## 2. mkdocs

> **Install mkdocs using pip** (need to repeat it for each user)
> 
> See detailed instructions in [**mkdocs-material official site**](https://squidfunk.github.io/mkdocs-material/)

```bash
# 1. Intall mkdocs for each user
pip install mkdocs-material

# 2. Install more plugins for each user
pip install mkdocs-glightbox mkdocs-video mkdocs-audio mkdocs-callouts mkdocs-redirects
# pip install mkdocs-encryptcontent-plugin

# 3. Setup shortcuts in ~/shortcuts for each user

```