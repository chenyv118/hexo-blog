---
title: Hello Hexo
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

## Hexo博客搭建

### Hexo安装
```npm install hexo-cli -g```

### 初始化博客
```hexo init [文件夹名字]```

### 安装依赖
```npm install```

### 预览
```hexo s```

## 部署到github
### 配置git
``` bash
git config --global user.name "chenyv118"
git config --global user.email "3241218997@qq.com"
```

### 本地配置
打开项目根目录中的_config.yml文件，找到deploy
``` bash
deploy:
  type: 'git'
  ### 使用https就可以不用配置ssh密钥
  repo: 'https://github.com/chenyv118/chenyv118.github.io.git'
  ### repo: 'git@github.com:chenyv118/chenyv118.github.io.git'
  branch: main
```
右下角可以切换换行符为```CRLF```或```LF```

### 安装部署插件
```npm install hexo-deployer-git --save```

## 设置模板

### 安装
```npm install hexo-butterfly-cli -g```

### 使用
```butterfly-cli init [projectName]```

### 安装依赖
```
cd [projectName]
npm install
```

## Butterfly主题
### 安装主题
```npm install hexo-theme-butterfly```

### 应用主题
修改 Hexo 根目录下的 _config.yml，把主題改为butterfly
```theme: butterfly```

### 安装插件
如果沒有 pug 以及 stylus 的渲染器，請下載安裝：
```npm install hexo-renderer-pug hexo-renderer-stylus --save```

### 升级建议
在 hexo 的根目錄創建一個文件 _config.butterfly.yml，並把主題目錄的 _config.yml 內容複製到 _config.butterfly.yml 去。( 注意: 複製的是主題的 _config.yml ，而不是 hexo 的 _config.yml

## 版本控制
备份博客，便于电脑出故障也能够保证博客不会丢失。

### git初始化
```git init```

### 远程推送
提交到本地仓库  
```git commit -m "first commit"```  
推送到远程  
```git branch -M main```  
```git remote add origin https://github.com/chenyv118/hexo-blog.git```  
```git push -u origin main```

## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
