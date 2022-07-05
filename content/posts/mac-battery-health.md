---
title: "MacBook Pro 電池健康情況檢查"
subtitle: ""
date: 2021-11-05T19:14:16+08:00
draft: false
author: "DevenTW"
description: "Check Your Mac Battery Health!"

tags: ["mac","macbook","battery"]
categories: ["Sharing"]


---

![Laptop Image](https://images.unsplash.com/photo-1583863788434-e58a36330cf0?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1074&q=80)
<!--more-->

<!--more-->

## MacBook Pro 電池健康情況查詢

2018 年 9 月入手的 Macbook Pro 13,
檢查了一下電池🔋的損耗情況。

## 檢查方法

在 terminal 輸入下方指令：

```bash
ioreg -rn AppleSmartBattery | grep -i capacity

```

## 運行結果

- "AppleRawCurrentCapacity" = 1839
- "AppleRawMaxCapacity" = 4313
- "MaxCapacity" = 4313
- "CurrentCapacity" = 1839
- "CycleCount"= 182
- "DesignCapacity" = 5088

"AppleRawCurrentCapacity" = 4337
"AppleRawMaxCapacity" = 4371
"MaxCapacity" = 4371
"CurrentCapacity" = 4337
"DesignCapacity" = 5088

DesignCapacity 是設計的最大電池容量 -> 5088
MaxCapacity 是電池實際容量 -> 4371/4337

CycleCount 是電池循環的次數 -> 182，
大家也不妨測試一下自己的 Mac 電池狀況。
