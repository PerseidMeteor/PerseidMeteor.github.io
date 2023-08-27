---
layout: post
title: CS、IO、事件处理
subtitle: test
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [linux, network]
---

# CS、IO、事件处理

---



## 1.C/S模型

![image-20230212153911774](/assets/img/image-20230212153911774.png)

缺点：当访问量过大时，客户端可能需要很长时间才能获得服务

## 2.P2P模型

![image-20230212154335359](/assets/img/image-20230212154335359.png)

缺点：用户之间传输请求过多时，网络负载会加重



## 3.IO模型



## 4.事件处理

**`Reactor模式`**

![image-20230212155837964](/assets/img/image-20230212155837964.png)

>Reactor模式主线程上等待监听/连接socket，socket的读写以及业务逻辑则是交给了工作线程完成。
>
>
>
>



**`Proactor模式`**

![image-20230212160959382](/assets/img/image-20230212160959382.png)

>Reactor模式主线程上等待监听/连接socket，IO事件则是交给了内核执行，工作线程只负责业务逻辑