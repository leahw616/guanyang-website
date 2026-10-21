# 冠阳公司网站 · Guanyang Website

5 个页面（首页 / 公司简介 / 产品介绍 / 生产设备 / 联系我们），
5 种语言一键切换：English · 中文 · Español · Français · 日本語。

## 文件结构

```
index.html          首页
about.html          公司简介
products.html       产品介绍
factory.html        生产设备与品控
contact.html        联系我们
assets/css/style.css
assets/js/i18n.js   五语言翻译字典 + 语言切换逻辑
assets/img/         网站图片（来自公司简介 PPT，已压缩）
```

## 本地预览

用浏览器打开 `index.html` 即可；推荐起一个本地服务（避免 file:// 限制）：

```bash
cd guanyang-site && python3 -m http.server 8000
# 浏览器访问 http://localhost:8000
```

## 发布到 GitHub Pages

1. 在 GitHub 新建一个仓库（例如 `guanyang-website`），把本文件夹所有文件上传到 `main` 分支根目录
2. 进入仓库 **Settings → Pages**
3. Source 选择 **Deploy from a branch**，Branch 选 `main`，目录选 `/ (root)`，保存
4. 等 1–2 分钟，访问 `https://<你的用户名>.github.io/<仓库名>/` 即可

## 国内访问说明

- GitHub Pages 在国内一般可以打开，但速度不稳定、偶尔偏慢。
- 网站本身已按国内可访问标准构建：**零外部请求**（无 Google Fonts、无境外 CDN，全部使用系统字体与本地文件），放在任何国内服务器/CDN 上都能正常打开。
- 如果国内客户访问速度是重点，可以考虑：Cloudflare Pages（免费、全球 CDN）、阿里云 OSS + CDN、腾讯云静态网站托管。需要的话我可以帮你评估。

## 待补充

- **联系电话 / 邮箱**：目前联系页为占位符（"(待补充)"），请提供真实联系方式，我来填上。
- **产品详细介绍**：等你发抖音链接，我把具体产品信息补充到产品页。
