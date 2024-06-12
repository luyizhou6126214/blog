---
title: 记录docker compose部署问题
date: 2024-06-12 21:15:04
tags: docker
categories:
- 问题记录
---

# 问题描述

docker compose配置文件中，通过command命令启动sh脚本，但是docker服务没法启动，一直重试中





# 解决方案

shell脚本中，加一行

```shell
tail -f /dev/null
```

参考：https://segmentfault.com/q/1010000044675593
