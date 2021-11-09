---
title: "Git Ssh"
date: 2021-10-17T16:27:54+08:00
draft: false
images: []
tags: ["工具"]
---

# git 使用ssh密钥

## 生成ssh密钥

```ssh-keygen -t ed25519 -C "your_email@example.com"```

## ssh-agent管理密钥

```
# 手动启动ssh-agent
$ eval "$(ssh-agent -s)"
> Agent pid 59566
# 将ssh私钥添加到ssh-agent
$ ssh-add ~/.ssh/id_ed25519
```

```将公钥存放至github```
