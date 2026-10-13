# CJProject

Web 前端实训项目 —— 一个多页面的静态站点，使用原生 HTML / CSS / JavaScript，未使用任何框架。

## 目录结构

```
index.html                     入口 / 登录页
DropletServicce.html           登录成功后的跳转页
MyDroplet.html                 我的
EnterpriseProjectGold.html     企业项目 · 金
EnterpriseProjectSilver.html   企业项目 · 银
EnterpriseProjectDiamonds.html 企业项目 · 钻石
PlatformMien.html              平台风采
ServiceProcess.html            服务流程
ExternalStyle.css              公共样式
Joggle.js                      XMLHttpRequest 封装的 AJAX 工具
Resource/                      图片等静态资源
```

## 说明

- 登录页收集账号 / 密码，经 `Joggle()` 以 `application/x-www-form-urlencoded`
  提交到 mock 接口；返回「登录成功」则跳转 `DropletServicce.html`，否则 `alert` 错误信息。
- `Joggle(method, url, opt, callback)` 是 `XMLHttpRequest` 的薄封装：
  自动拼接 mock 接口前缀、设置请求头、解析返回的 JSON 并回调其中 `data`。
- 纯静态页面，直接用浏览器打开 `index.html` 即可预览（登录接口需联网）。

## 技术

HTML5 · CSS3 · 原生 JavaScript（DOM / XMLHttpRequest）

---

> 本 README 依据仓库现有代码整理，细节如与实现不符请以代码为准。
