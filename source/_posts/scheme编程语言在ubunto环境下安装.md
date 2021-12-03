---
title: scheme编程语言在ubunto环境下安装
date: 2021-12-02 17:02:30
category:
	scheme
tags:
	scheme
---

安装命令
```bash
sudo apt-get install mit-scheme
```

### 1.进入命令行交互：
```bash
scheme
```

### 2.加载文件：
vi test.scm, 输入以下代码，wq保存

```scheme
(write (+ 10 10))
```

进入交互模式，执行以下命令
```
(load "test.scm")
```