---
title: "Go 变量"
subtitle: "Go学习笔记"
date: 2019-08-03T16:42:15+08:00
tags: ["go"]
categories: “language”
nocomment: true
postmeta: false
notoc: ture
draft: false
---

#### 使用var关键字

* var a, b, c bool

* var s1, s2 string = "hello", "world"

* 可定义在函数体内或直接定义在包内

* 使用var()集中定义变量

  > ``` var ( a, b, c) ```

#### 编译器自动识别类型

* var a, b, i, s1, s2 = true, false, 1, "hello", "world"

#### 使用:=定义

* a, b, i, s1, s2 := true, false, 1, "hello", "world"
* 只能在函数体内定义使用