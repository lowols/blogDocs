---
title: git操作笔记
tags:
  - 文档编辑
categories:
  - 编程软件
date: 2025-12-8 15:52:59
---



## 多账户配置

电脑已有一个git账户，想添加一个新账户。

1. 生成秘钥文件（例如文件名：id_rsa.github），并将公钥加入到云仓库中的keys中

   ```
   ssh-keygen -t rsa -f ~/.ssh/id_rsa.github -C "邮箱"
   ```

   ```
   Github：
   https://github.com/settings/keys
   ```

   

2. 在~/.ssh下创建config文件，并写入以下内容

```
Host github.com
    HostName github.com
    User git
    IdentityFile ~/.ssh/
```



### 图片

1. 可以将文件中所有图片统一移动至某个文件夹

