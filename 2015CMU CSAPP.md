---
title: CMU CS:APP笔记#1
category: cs
tag: 
 - csapp
id: 12
date: 2023-9-12
---

## Bits,Bytes, and Integer

#### Logic Operations inC

在讲到这一部分内容时，PPT上展示了一个例子

```c
p && *p //avoid null pointer access
```

这个例子很有趣，因此记录下来分析一下。

&& 运算符是一个惰性运算符，只要第一个值为0或者NULL，那么后面的值就不需要计算，因此，就可以做到在解引用指针p之前先判断p是否为空指针。这样就避免了对空指针的引用。

