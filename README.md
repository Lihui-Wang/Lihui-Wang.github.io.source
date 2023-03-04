# Quick Start

1. ``Hugo -S``生成``public``文件夹
2. 同步到``github.io.source``：``git add -A && git commit -m "trying action 3" && git push -u origin main``

# Hugo

[Hugo + GitHub Pages 搭建自己的网站](https://blog.csdn.net/azl397985856/article/details/110848517)

[Hugo官网](https://gohugo.io/getting-started/quick-start/)

## Theme

### [Academic](https://sourcethemes.com/academic/)

[Edit on your PC with Hugo Extended](https://wowchemy.com/docs/getting-started/install-hugo-extended/)

```
# 安装 Go 依赖
sudo snap install --classic go

# 下载 Academic 主题, 有 bug，主题、slider和地图无法正确显示
# git clone https://github.com/wowchemy/starter-academic.git
# cd starter-academic

# 下载 Academic research group 主题
git clone https://github.com/wowchemy/starter-hugo-research-group
cd starter-hugo-research-group-main

# https://wowchemy.com/docs/getting-started/install-hugo-extended/
在中国
If you are in China without VPN, Hugo can fail to download modules from GitHub.
To resolve this, you can try adding a proxy to the module section of your config/_defaults/config.yaml:
module:
  proxy: https://goproxy.cn

# 打开测试服务器
hugo server

# 通过 Hugo 生成静态页面，默认 public
hugo -D

# 通过 Hugo 生成静态页面时，指定目标目录为 docs：
hugo -d docs

```
- Academic research group 这个主题比较特殊，必须把内容放在根目录，否则 Github 的 action 会失败
- Academic research group 开发文档：https://wowchemy.com/docs/getting-started/page-builder/

```bash
# 先下载测试，build
git clone https://github.com/wowchemy/starter-academic.git
cd starter-academic
# 发开服务器, -D include content marked as draft, -w watch filesystem for changes and recreate as needed
hugo server -D -w
hugo -D
```
- 然后移动到根目录，不用合并``.git``,``.github``,``readme.MD``等文件/文件夹
- 删除原 starter-academic 文件夹
- 这样以后更新时，只要用``hugo -D``命令 build 到``public``文件夹后，然后 push 到 github.io.source 即可以通过 action 同步到 github.io

# Github
[折腾Hugo | GitHub Pages | Github Actions自动构建发布免费个人网站](https://zhuanlan.zhihu.com/p/109057290)

```bash
# 生成 ssh，用于 githubio.source 向 githubio 同步
ssh-keygen -t rsa -b 4096 -C "jakkwj@github.io"
# 注意修改文件夹位置存放 ssh key
/home/gift/Desktop/12311111/id_rsa_hugo_deploy
# passphrase 必须为空
```
- 去 github.io 库 -> setting -> Deploy key 添加 Public Key，注意首尾空格也要 copy
  - Title: public key of source code
  - Key: 上面生成的pub
  - Allow write access: √
- Private Key 添加到 github.io.source 库，注意首尾空格也要 copy
  - 这里 Secrets 变量名要一定: ACTIONS_DEPLOY_KEY
  - ACTIONS_DEPLOY_KEY那里要把"-----BEGIN OPENSSH PRIVATE KEY-----"这些都写进去
- 为 github.io.source 仓库配置 Actions
```bash
name: Deploy Hugo Site to Github Pages on Main Branch

on:
  push:
    branches:
      - main

jobs:
  build-deploy:
    # runs-on: ubuntu-18.04
    runs-on: ubuntu-latest
    steps:
      # - uses: actions/checkout@v2
      - uses: actions/checkout@v1  # v2 does not have submodules option now
       # with:
       #   submodules: true

      - name: Setup Hugo
        uses: peaceiris/actions-hugo@v2
        with:
          hugo-version: '0.92.2'  # 注意版本
          # extended: true

      - name: Build
        #run: hugo --minify
        run: |
          cd starter-academic
          hugo --minify

      - name: Deploy
        uses: peaceiris/actions-gh-pages@v3
        with:
          deploy_key: ${{ secrets.ACTIONS_DEPLOY_KEY }} # 这里的 ACTIONS_DEPLOY_KEY 则是上面设置 Private Key的变量名
          external_repository: jakkwj/jakkwj.github.io # Pages 远程仓库
          # publish_dir: "./starter-academic/public/"
          publish_dir: "./public/"
          keep_files: true # remove existing files
          publish_branch: main  # deploying branch
          commit_message: ${{ github.event.head_commit.message }}

```
- 添加了 Acitons 后, 会自动生成一个网页 push 生成 .github/workflows/main.yml, 此时要先 ``git pull origin main`` 一次, 然后才能正常 push, 否则会出现以下错误:
  - 如果出现了``如何解决更新被拒绝，因为远程版本库包含您本地尚不存在的提交。``等提示, 此时需要强制执行``git push -u origin +master``
- publish_dir: "./public/"，只发布hugo生成的public目录
- keep_files: true，不删除原有仓库的文件，对于需要保留自定义域名CNAME文件等情

## 注意
- 生成 ssh key 时, passphrase 必须为空, 否则 action build 会卡这里失败
- 修改了 action 的 .github/workflows/main.yml, 需要先**在根目录下** ``git pull origin main`` 一次
- docs文件夹一直不成功: ~~数据源默认使用主分支下的根目录，我个人建议改为 docs 目录；~~
- 小细节：避免 Jekyll 起作用，可以在仓库根目录放一个空文件，文件名：.nojekyll

# Academic主题开发

## 多语言

- https://wowchemy.com/docs/hugo-tutorials/language/

- ``content``文件夹下分``en``、``zh``2个文件夹，``zh``可以先复制``en``一样的内容，然后在翻译成中文

-  ``config.yaml``修改
  - ``baseURL: 'https://usernamexxxx.github.io/'``
  - 默认语言：``defaultContentLanguage: en``

- 语言在``languages.yaml``中设置

## 路由
- 默认语言的路由在``meaus.yaml``中设置
- 非默认语言的路由在``languages.yaml``的``menu``进行设置







