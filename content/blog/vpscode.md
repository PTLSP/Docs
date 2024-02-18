---
title: 我的VPS常用命令（长期更新）
date: 2024-01-10 0:06:03
updated: 2024-01-10 0:06:03
swiper_index: 1 

description: 我的VPS常用命令（长期更新）

cover: https://vps234.oss-cn-shanghai.aliyuncs.com/Content/2-2021/2021-6-10/1.jpg

permalink: /vpscode/

tags: 
- 长期更新
- 代码
- 自用
categories: 
  - Server
---

## 查看Linux 系统信息 网络带宽及硬盘读写速率

官网：https://bench.sh/
```bash
wget -qO- bench.sh | bash
```
或
```bash
curl -Lso- bench.sh | bash
```
## 测试流媒体服务解锁状态

Github：https://github.com/lmc999/RegionRestrictionCheck

只检测IPv4结果：
```bash
bash <(curl -L -s check.unlock.media) -M 4
```
只检测IPv6结果：
```bash
bash <(curl -L -s check.unlock.media) -M 6
```
## 一键查看解锁Chatgtp命令
```bash
bash <(curl -Ls https://cdn.jsdelivr.net/gh/missuo/OpenAI-Checker/openai.sh)
```
宝塔面板Ubuntu/Deepin安装脚本
```bash
wget -O install.sh https://download.bt.cn/install/install-ubuntu_6.0.sh && sudo bash install.sh ed8484bec
```
## x-ui修改版一键脚本（xray内核）

Github地址：https://github.com/yonggekkk/x-ui-yg
```bash
bash <(wget -qO- https://gitlab.com/rwkgyg/x-ui-yg/raw/main/install.sh 2> /dev/null)
```
或
```bash
bash <(curl -Ls https://gitlab.com/rwkgyg/x-ui-yg/raw/main/install.sh)
```


