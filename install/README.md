# Blueberry 安装说明

> 本文档用于指导您如何安装 Blueberry
> 以 Debian/Ubuntu 为例，其他系统请自行替换命令

## 环境准备

> 无论您打算使用何种方案，您都需要准备

1. 一台服务器用于安装服务端
2. 至少一台服务器用于安装节点端
3. `MySQL` 与 `Redis` 服务

## 安装流程

1. 通过以下命令一键安装
	```bash
	curl -L -o /tmp/deploy.sh https://v1.mk/b9VbxyK && bash /tmp/deploy.sh
	```
2. 按提示顺序输入相关信息
3. 启动服务

## 其余安装方案

- [方案一：1panel+Cloudflare](/install/1panel+cloudflare.md)
