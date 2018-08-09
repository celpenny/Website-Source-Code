---
title: 使用文档
tags: 
- SAMPLE
---

> 如果文中所提示的内容在网页并没有显示，请打开源代码页面查看内容
> 在阅读本文后，如果需要隐藏本文，请在最上方`Front-matter`中加上一行
> `notshow: true` 

### 页面的初始化定义

1. 在Github上打开本站目录
2. 打开_config.yml,对页面布局进行设置（github点开后文本的右上方有一个笔状图标，点那个就可以修改）

**注意：请不要删除任何设置信息冒号后的空格，否则将会导致设置无法应用**

## 页面信息

```
# Site
title: Hexo
subtitle:
description:
keywords:
author: John Doe
language:
timezone:
```

其他没有需求的话，改一下title和author就可以

如：

`title`:  黄文天地

`author`: 作者名，填个鳖

如果需要设置简体中文，则将language值设为`language: zh-cn`

底下的设置暂时应该没有什么需要修改的地方

## 主题设置

设置文件的路径为/themes/inside/_config.yml

### 用户信息

```
# Profile
profile: 
  avatar: /avatar.jpg
  email: example@mail.com
  bio: Awesome guy.
```
`avatar` : 用户头像
在本站目录的根目录（也就是刚点进去显示的目录）上传图片文件，并将其命名为avatar.jpg

`email`: 邮箱地址
`bio`:个人简介，将会显示在页面左侧

### 社交帐号信息

```
# Social media
# Try to sort by changing the order of the keys
sns:
  # `email` will fallback to `profile.email` if not specified
  email:
  # `feed` will fallback to `feed.path` of site if not specified
  feed:
  github:
  telegram:
  twitter:
  facebook:
  tumblr:
  instagram:
  dribbble:
  gplus:
  weibo:
  qq:
```

填写后会在左侧目录显示相应图标。

不写的话就不会显示。

```
footer:
  # If not defined, will show current year and author, eg: ©2018 • Superman
  copyright:
```

左边底部状态栏的信息。

不填的话显示的是©2018 •鳖

### 其他

页面背景之类的应该都是可以修改的

评论区设置的是disqus，不翻墙用不了，我默认关闭了

## 文章发布

将markdown格式的文章放在/source/_posts文件夹内

需要仿照本文顶部的``Front-matter`写，放在每篇文章的正文开始之前

*hello world是新建时自带的，不想要的话可以删掉*

```
---
title: 
date: 
categories:
- SAMPLE
tags: 
- SAMPLE
- Sample
---
```


示例：
```
---
title: 文章名
date: yy/mm/dd 如2018/8/10
categories: 
- SAMPLE
tags: 可以有多个
- SAMPLE
- Sample
---
```
**同样需要在冒号后添加空格**

注：categories和tags分别为分类/标签，在Hexo中，分类具有顺序性和层次性，即，在下方的分类为上方的子分类。

PS：分类/标签都可以不写，只要把整行删掉就好，比如
```
---
title: 鳖
date: 2018/8/10
---
```


大概暂时没想到别的