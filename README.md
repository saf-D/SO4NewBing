# SO4NewBing

基于微软 New Bing 简单定制，拥有一致的 UI 体验，支持 ChatGPT 提示词，国内可用，基本兼容微软 Bing AI 所有功能，无需登录即可畅聊。

⭐ 国内可用 （部署服务器需要直连 www.bing.com 不重定向 CN ，可配置 socks 连接）

⭐ 支持现有开源提示词库

⭐ 需要画图等高级功能时，可登录微软账号设置用户 Cookie 进行体验

⭐ 遇到一切问题，先点左下角 ![新主题](./docs/img/bing-clear.png) 试试，不行使用刷新大法（Shift + F5 或 Ctrl + Shift + R 或 右上角设置中的一键重置），最终大招就 清理浏览器缓存 及 Cookie ，比如（24 小时限制、未登录提示等等）

MENU
- [go-proxy-bing](#go-proxy-bing)
  - [网页展示](#网页展示)
  - [侧边栏](#侧边栏)
  - [演示站点](#演示站点)
  - [获取 Cookie](#获取Cookie)
  - [环境变量](#环境变量)
  - [部署](#部署)
    - [Docker](#Docker)
    - [Release](#Release)
    - [Railway](#Railway)
    - [Vercel](#Vercel)
    - [Render](#Render)
  - [TODO](#TODO)

## 网页展示

- 电脑端未登录状态

![电脑未登录](./docs/img/bing-nologin.png)

- 电脑端登录

![电脑端登录](./docs/img/bing-login-1.png)
![提示词1](./docs/img/bing-prompt-1.png)
![提示词2](./docs/img/bing-prompt-2.png)

- 电脑端画图

> ⭐ 需登录，并选择 更有创造力 对话模式

![电脑端画图](./docs/img/bing-draw.png)

- 手机端未登录状态

![手机端未登录](./docs/img/bing-m-nologin.png)

## 侧边栏

- 在 Edge 浏览器可把聊天和撰写分别添加侧边栏

![添加侧边栏](./docs/img/sidebar-add.png)

![聊天](./docs/img/sidebar-chat.png)

![撰写](./docs/img/sidebar-compose.png)

## 站点大全

### Vercel通道

- https://so-4-new-bing-saf-d.vercel.app/

- https://so4ai.vercel.app/

- https://hiso4.vercel.app/

- https://1145141.vercel.app/

- https://so4-bing.vercel.app/

- https://new-bing.vercel.app/

- https://so4-newbing.vercel.app/

### Render 搭建

- https://go-proxy-bingai-uciv.onrender.com/

- https://so4.流浪地球.xyz/

## 获取 Cookie

- 访问 https://www.bing.com/ 或 https://cn.bing.com/ ，登录

- F12 或 Ctrl + Shift + I 打开控制台

- 拿到 Cookie 后，在网站设置用户 Cookie 弹窗填入即可。

![获取Cookie](./docs/img/bing-cookie.png)

## 环境变量

```bash
# 运行端口 默认 8080 可选
PORT=8080
# Socks 环境变量 示例 可选
Go_Proxy_BingAI_SOCKS_URL=192.168.0.88:1070
# Socks 账号、密码 可选
Go_Proxy_BingAI_SOCKS_USER=xxx
Go_Proxy_BingAI_SOCKS_PWD=xxx
# 默认用户 Cookie 设置，可选，固定前缀 Go_Proxy_BingAI_USER_TOKEN 可设置多个，未登录用户将随机使用
Go_Proxy_BingAI_USER_TOKEN_1=xxx
Go_Proxy_BingAI_USER_TOKEN_2=xxx
Go_Proxy_BingAI_USER_TOKEN_3=xxx ...
```

## 部署

见https://github.com/adams549659584/go-proxy-bingai
