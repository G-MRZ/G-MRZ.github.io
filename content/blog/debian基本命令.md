---
title: "Debian基本命令"
date: 2021-11-09T22:35:39+08:00
draft: false
images: []
tags: ["linux"]
---

### debian/Ubuntu命令

| apt              | apt-get              | 作用                           |
| ---------------- | -------------------- | ------------------------------ |
| apt install      | apt-get install      | 安装软件包                     |
| apt remove       | apt-get remove       | 移除软件包                     |
| apt purge        | apt-get purge        | 移除软件包及配置文件           |
| apt update       | apt-get update       | 刷新存储库索引                 |
| apt upgrade      | apt-get upgrade      | 升级所有可升级的软件包         |
| apt autoremove   | apt-get autoremove   | 自动删除不需要的包             |
| apt full-upgrade | apt-get dist-upgrade | 在升级软件包时自动处理依赖关系 |
| apt search       | apt-cache search     | 搜索应用程序                   |
| apt show         | apt-cache show       | 显示装细节                     |

```Shell
sudo update-alternatives --config editor # 配置默认文本编辑器
sudo update-alternatives --config x-terminal-emulator # 配置默认终端
echo $SHELL # 显示当前shell
cat /etc/shells # 显示所有安装的shell
chsh # 配置默认shell
```

