---
title: vscode安装golang插件报错Installing github.com/ramya-rao-a/go-outline@latest FAILED
date: 2022-04-26 22:51:52
category:
	- go
tags:
    - go
---
先查看一下gopath 目录在哪
```bash
go env|grep GOPATH
GOPATH="/Users/xiaoma/go"
```


```bash
mkdir -p /Users/xiaoma/go/src/golang.org/x/
 
cd /Users/xiaoma/go/src/golang.org/x/
 
git clone https://github.com/golang/tools.git
 
export GOPROXY=https://goproxy.cn,direct
```

然后重启你的 vs code，再进行install all 就行了。