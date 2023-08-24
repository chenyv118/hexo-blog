---
title: butterfly主题的使用
date: 2023-08-24 12:21:43
tags:
---
## 基本配置
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

## 页面配置

### 标签页
进入根目录，输入如下命令  
```hexo new page tags```  
于是得到了文件```source/tags/index.md```  
添加```type: "tags"```

### 分类页
进入根目录，输入如下命令  
```hexo new page categories```  
于是得到了文件```source/categories/index.md```  
添加```type: "categories"```

### 友情链接
进入根目录，输入如下命令  
```hexo new page link```  
于是得到了文件```source/link/index.md```  
添加```type: "link"```  
在Hexo博客目錄中的 ```source/_data```（如果沒有 _data 文件夾，請自行創建），創建一個文件 ```link.yml```

### 404页面
主題內置了一個簡單的 404 頁面，可在設置中開啟  
在主题的配置页面中找到如下配置：
```markdown
# A simple 404 page
error_404:
  enable: false
  subtitle: "頁面沒有找到"
  background: 
```
将```false```改为```true```即可