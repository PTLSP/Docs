---
title: MoviePilot企业微信推送之新手喂饭教程
date: 2024-02-01 08:07:53
updated: 2024-02-01 08:07:53
swiper_index: 1
description: MoviePilot企业微信推送之新手喂饭教程
permalink: /moviepilotwechat/
cover: https://tse1-mm.cn.bing.net/th/id/OIP-C.QFPeY4rmVvrG2aTfKX7HCAAAAA?w=240&h=180&c=7&r=0&o=5&dpr=2&pid=1.7
tags: 
- MoviePilot
categories: 
- 原创教程
---



## 教学指引

期间参考：

https://pt-helper.notion.site/50a7b44e255d40109bd7ad474abfeba5

https://github.com/Putarku/MoviePilot-Help?tab=readme-ov-file#%E5%BE%AE%E4%BF%A1%E9%80%9A%E7%9F%A5%E9%97%AE%E9%A2%98



大家点进去看 了解各个信息 代表什么意思 网上教程已经很详细了 基础的我就不再过多的重述 直接看我的截图 找到以下几个关键点 我用数字代表各个参数 大家理解起来事半功倍

以下为windows的配置文件参数 docker用户无需担心 对号入座进群晖docker 其实是一样的 主要就是这几个环境变量 别害怕 我会带领大家一步一步的操作并理解。

## 配置变量

- WeChat企业ID
  WECHAT_CORPID=①

- WeChat应用Secret
  WECHAT_APP_SECRET=②

- WeChat应用ID
  WECHAT_APP_ID=③

- WeChat代理服务器
  WECHAT_PROXY=④

- WeChat Token
  WECHAT_TOKEN=⑤

- WeChat EncodingAESKey
  WECHAT_ENCODING_AESKEY=⑥

### # WeChat企业ID

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/image026cf54236226777-20240201095607462.png)

### # WeChat应用Secret

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/image3d8d01d771a150a2-20240201095627891.png)

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/imagebde89f36ac779fbd-20240201095646769.png)

贴心附上MP的LOGO:

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/ikuf2u-20240201095748515.webp)



![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/image81883dea1920ee07.png)

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/image205a247007a37a12.png)

### # WeChat应用ID

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/imagebeee28b4ce025956.png)

### # WeChat代理服务器
我已经用我的vps搭建了代理服务器 并绑定了域名 大家直接调用就好

微信代理地址：https://mp.ptlsp.com/

企业微信应用后台的
企业可信IP：148.135.46.230

微信代理地址我想要大家长期使用 所以不需要再去mp配置参数里去改微信代理地址了 我已经把ip绑定到域名上了
就算以后vps到期 或者这个v4固定公网失效了 我会继续采购vps 绑定微信到代理地址 让大家继续用 只需要登录企业微信更换企业可信ip 为最新的IP即可！

避免期间大家翻车 我把细节交代清楚 看下面截图 准确填入！！！

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/1704504711352-20240201101547549.png)


ps：如果你是老版本 配置文件提示微信代理服务器最后面不需要添加 “/”  你都加不加都试一下嘛 这东西说不清楚 
我参考网上教程看到别人是加上的 我也加上的 我没问题 不行都试试 这个是个排错点 参考起来

###  WECHAT_TOKEN 跟 WeChat EncodingAESKey

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/3bbdc3900a59d76083fd81ddf4ce271.png)



![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/7ffb78e4b4b61cadd323129e764d502.png)



## 注意事项

期间tg用户反馈 跟着我的教程使用 http://ip:端口/api/v1/message/?token=moviepilot 这个接口导致MP开机即死机 连日志都看不到
他的环境为：群晖6.2 Docker
在我的建议下 他使用官方提供的第二个接口地址就成功了 所以我之前的教程也明说了 未知bug我也不懂 这两换着来 不要纠结！ 

```URL
http://ip:端口/api/v1/message/?token=moviepilot
```



```URL
http://ip:端口/api/v1/message/
```



切记二选一！！！！

### 官方解释

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/image27f84a7a6f37d008.png)

### 填写可信IP

```IP
148.135.46.230
```



![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/c701844fe3768d9498220ac53f20502.png)



自此 教程结束 完成以上步骤基本没问题了

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/image9c05b185eb43c7dd.png)

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/imagec983028c05e2058d.png)



![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/image3298fcf670bde9be.png)

MP系统版本参考：

![image](../img/2024-02-01-MoviePilot%E4%BC%81%E4%B8%9A%E5%BE%AE%E4%BF%A1%E6%8E%A8%E9%80%81%E4%B9%8B%E6%96%B0%E6%89%8B%E5%96%82%E9%A5%AD%E6%95%99%E7%A8%8B/image0e68798a3cea6087.png)



## 服务声明

{% tip ban faa-parent animated-hover %}<p class="faa-flash">不允许任何技术大佬利用此免费服务售卖技术！此教程不允许转载到国内任何公共平台 ！服务完全免费！仅供学习参考！</p>{% endtip %}

截止到2024.2.1 我未更新系统 依旧有效 如有问题 及时反馈！

Github服务地址：https://github.com/PTLSP/MoviePilot-Wechat-PROXY