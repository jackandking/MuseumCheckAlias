# MuseumCheckAlias - 博物馆打卡域名跳转

[English](#english) | [中文](#中文)

---

## 中文

### 项目简介

本项目是一个简单的域名跳转服务，用于将中文域名 **博物馆打卡.cn** (xn--9kroa195ivupp99b.cn) 重定向到主站 [museumcheck.cn](https://museumcheck.cn)。

### 功能说明

- **自动跳转**：访问 博物馆打卡.cn 时会自动跳转到 museumcheck.cn
- **路径保持**：404 页面会保持原始路径并跳转到主站对应页面
- **双重保障**：使用 HTML meta refresh 和 JavaScript 实现双重跳转机制
- **GitHub Pages托管**：基于 GitHub Pages 提供稳定的静态页面服务

### 域名说明

- **中文域名**：博物馆打卡.cn
- **Punycode编码**：xn--9kroa195ivupp99b.cn
- **目标域名**：museumcheck.cn

### 技术实现

1. **index.html**：首页立即跳转到主站
2. **404.html**：404 错误页面，保持路径参数并跳转
3. **_config.yml**：GitHub Pages 配置文件
4. **CNAME**：自定义域名配置

### 部署方式

本项目通过 GitHub Pages 自动部署，无需额外配置。任何推送到主分支的更改都会自动生效。

### 使用场景

这个项目适用于：
- 为中文域名提供便捷访问入口
- 统一多个域名到一个主站
- 保持 SEO 友好的域名重定向

---

## English

### Project Overview

This project is a simple domain redirect service that redirects the Chinese domain **博物馆打卡.cn** (xn--9kroa195ivupp99b.cn) to the main site [museumcheck.cn](https://museumcheck.cn).

### Features

- **Automatic Redirect**: Visitors to 博物馆打卡.cn are automatically redirected to museumcheck.cn
- **Path Preservation**: The 404 page preserves the original path and redirects to the corresponding page on the main site
- **Dual Mechanism**: Uses both HTML meta refresh and JavaScript for reliable redirection
- **GitHub Pages Hosting**: Provides stable static page service via GitHub Pages

### Domain Information

- **Chinese Domain**: 博物馆打卡.cn (Museum Check-in.cn)
- **Punycode Encoding**: xn--9kroa195ivupp99b.cn
- **Target Domain**: museumcheck.cn

### Technical Implementation

1. **index.html**: Home page with immediate redirect to main site
2. **404.html**: 404 error page that preserves path parameters during redirect
3. **_config.yml**: GitHub Pages configuration file
4. **CNAME**: Custom domain configuration

### Deployment

This project is automatically deployed via GitHub Pages. Any changes pushed to the main branch will take effect automatically.

### Use Cases

This project is suitable for:
- Providing convenient access through Chinese domain names
- Unifying multiple domains to a single main site
- Maintaining SEO-friendly domain redirects

---

## License

This project is for domain redirection purposes only.

## Contact

For questions about the main Museum Check-in service, please visit [museumcheck.cn](https://museumcheck.cn).
