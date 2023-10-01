# Blueberry 安装说明

> 本文档用于指导您如何安装 Blueberry
> 以 Debian/Ubuntu 为例，其他系统请自行替换命令

## 环境准备

> 无论您打算使用何种方案，您都需要准备

1. 一台服务器用于安装服务端
2. 至少一台服务器用于安装节点端

## 安装方案

### 方案一：1panel+Cloudflare

> 本方案最简单省事

#### 准备

1. 准备 需要您拥有一个域名，且您的域名需要支持 Cloudflare


#### 安装流程

> 假设您的域名为 `blueberry.org`

1. 安装 [1panel](https://1panel.cn/)，参考[安装文档](https://1panel.cn/docs/installation/online_installation/)
2. 登录 1panel 进入 `应用商店`，安装 `MySql`、`Redis`，并记住相关密码
3. 等待安装完成后，打开 `数据库` -> `创建数据库` ，填入`名称`、`用户名`、`密码`并记住，点击 `创建`
4. 进入服务器控制台，输入 `curl -L -o /tmp/deploy.sh https://v1.mk/b9VbxyK && bash /tmp/deploy.sh` 以开始安装 `Blueberry`
   1. 按提示分别输入相关信息
   2. 如您选择的默认设置，缓存地址可以使用默认配置。缓存连接密码填入 `Redis` 的密码
   3. 如您选择的默认设置，数据库配置中的地址。端口可以直接选择默认，将 `步骤3` 中的`名称`填入`库名`，`用户名`填入`用户名`，`密码`填入`密码`
   4. 监听地址于监听端口可使用默认配置
   5. 服务域名请填入 您的域名（如：`https://blueberry.org`)
