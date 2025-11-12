# MkDocs and Jeyll - making webpages in MacOS

> **Install MkDocs ( prerequisite: [pip](./homebrew.md#2-python-pip) )**
> 
> **Install Ruby, Jekyll/Github Pages ( prerequisite: [homebrew](./homebrew.md) )**


## mkdocs

> **Install mkdocs using pip** (need to repeat it for each user)
> 
> See detailed instructions in [**mkdocs-material official site**](https://squidfunk.github.io/mkdocs-material/)

```bash
# 1. Intall mkdocs for each user
pip install mkdocs-material

# 2. Install more plugins for each user
pip install mkdocs-glightbox mkdocs-video mkdocs-audio mkdocs-callouts mkdocs-redirects
# pip install mkdocs-encryptcontent-plugin

# 3. Setup shortcuts in ~/.shortcuts for each user

```


## ruby/chruby

> **Insall ruby/chruby using brew** 
> 
> ruby is a prerequisite of Jekyll (see Jekyll's [Quickstart](https://jekyllrb.com/docs/) )

```bash
# 1. install ruby using ruby-install (one time for all users)
brew install chruby ruby-install
ruby-install ruby 3.4.1

# 2. then, add these to .zprofile for each uesr
source /opt/homebrew/opt/chruby/share/chruby/chruby.sh
source /opt/homebrew/opt/chruby/share/chruby/auto.sh
chruby ruby-3.4.1
```



## Jekyll/Github Pages

> **Insall Jekyll using ruby/gem**
> 
> See detailed instructions in [**Jekyll official site**](https://jekyllrb.com/)

```bash
# 1. Install jekyll (may need to repeat it for each user, not tested yet)
gem install jekyll
gem install jekyll bundler

# 2. Setup shortcuts in ~/.shortcuts for each user

```

