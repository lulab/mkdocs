# Homebrew & Pip in MacOS

> **Install homebrew, python, pip**


##  1.homebrew

### Step 1. Installation

```bash
## option A. Chinese mirror site (one time for all users)
/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"

## option B. Official site (need FQ)(one time for all users)
/bin/bash -c “$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)”
```

### Step 2. Permissions

>  **Setup permissions and env. for multiple users/accounts**
 
```bash
## Step 2.1) Setup permissions for multiple users in admin group
sudo chgrp -R admin /opt/homebrew ; sudo chmod -R ug+w /opt/homebrew ; sudo chmod -R a+rX /opt/homebrew

## Step 2.2) add these to ~/.zprofile for each user's account
eval $(/opt/homebrew/bin/brew shellenv) 

## Step 2.3) if installed brew using tsinghua mirror site, add these to ~/.zprofile as well
export HOMEBREW_PIP_INDEX_URL=https://pypi.tuna.tsinghua.edu.cn/simple 
export HOMEBREW_API_DOMAIN=https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles/api  
export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.tuna.tsinghua.edu.cn/homebrew-bottles 
```

### Update/Upgrade

> update and upgrade brew if too old 

```bash
brew update
brew upgrade
```


## 2. python & pip

### Install python using brew

**Installation**

`brew install python`


**Upgrade**

```
brew update
brew upgrade python
brew link --overwrite python
```


###  Setup pip with python

> **note:** 
>
> need to repeat the following for each user
> 
> command `pip` seems different from command `pip3` 


#### **Option 1**
 
```bash
### Step 1
python3 -m pip install --upgrade pip
# or
/Library/Developer/CommandLineTools/usr/bin/python3 -m pip install --upgrade pip

### Step 2a: add this to .zprofile 
export PATH="$HOME/Library/Python/3.9/bin:$PATH"

### Step 2b: may also try this instead of 2a (not tested yet)
brew unlink python && brew link python
```

#### **Option 2** (if option 1 not working) 

```bash
### Step 1
mkdir ~/venv
python3 -m venv ~/venv
# python3 -m pip install --upgrade pip

### Step 2a
### add this to ~/.zprofile
export PATH="$HOME/venv/bin:$PATH"
# pip install xyz

### Step 2b (if 2a not working)
source ~/venv/bin/activate
# python3 -m pip install xyz
```
 
