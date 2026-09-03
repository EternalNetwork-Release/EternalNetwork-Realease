# Eternal Network · 服务评估页

一个面向 GitHub Pages 的静态服务说明页。首屏先列出线路、流媒体、客户端和支持渠道，后面附上常见外网服务入口，方便访客快速判断是否适合自己。

## 页面内容

- 线路与内容：低价 IEPL 专线、YouTube / Netflix / Disney+ / Spotify 等流媒体访问
- 多平台客户端：Windows、macOS、Android、Linux、OpenWrt，iOS 使用 Shadowrocket 和共享小火箭账号
- 连接方式：订阅一键导入、自动更新、TUN / 规则 / 全局模式、校园网 / 内网模式、路由级代理
- 外网清单：搜索、AI、开发、科研、社交、兴趣、隐私、内容平台与 civitai，页面提供对应网站链接或平台说明
- 社区支持：官网文档、活跃工单与 [Telegram 群聊](https://t.me/Etcloud)，可直接联系群主和管理员
- 主题：默认白色，可在右上角切换黑色模式
- 字体：通过 Google Fonts 加载 Google Sans，并保留系统字体回退

## 本地预览

直接打开 `index.html`，或运行任意静态文件服务器：

```bash
python -m http.server 8000
```

页面不依赖构建工具，适合直接部署到 GitHub Pages。

> 内容来源：Eternal Network 使用文档（抓取时间：2026-09-01）。页面不展示客户端文件直链，客户端请从官网进入。

公开站点抓取记录保存在 `.site-crawl/`（已被 `.gitignore` 忽略）。抓取时官网返回 Cloudflare 403，因此价格仍以官网实时套餐页为准。


