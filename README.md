# 掌玩人才发展项目 · 官网

一个零依赖的静态网站，纯 HTML/CSS/JS，无构建步骤、无外部资源（图片与图标均已内联）。

## 目录结构

```
.
├── index.html          # 首页（GitHub Pages 默认入口）
└── pages/
    ├── about.html      # 认识掌玩 / 公司与项目
    ├── development.html# 计划与培养
    ├── culture.html    # 平台与文化
    ├── join.html       # 成长与加入
    ├── programs.html   # 三大计划（跳转到 development）
    ├── positions.html  # 实践平台（跳转到 culture）
    └── stories.html    # 成长见证（跳转到 join）
```

首页与子页之间可双向跳转：首页导航/按钮进入子页，子页导航与品牌标志返回首页对应板块。

## 部署到 GitHub Pages

1. 在本仓库的 **Settings → Pages** 中，将 Source 设为 **Deploy from a branch**。
2. Branch 选择 `main`，文件夹选择 `/ (root)`，保存。
3. 等待部署完成，访问 `https://division19.github.io/PP/`。

> 因为仓库名是 `PP`，站点地址带 `/PP/` 子路径。本站点所有链接都使用**相对路径**，因此在该子路径下可正常工作；本地直接双击 `index.html` 打开也能正常跳转。

## 本地预览

任选其一：

- 直接双击 `index.html` 打开；
- 或在本目录运行 `python -m http.server 8000`，然后访问 `http://localhost:8000`。

## 功能特性

- 浅色 / 深色主题切换（记忆用户选择，跟随系统偏好）
- 手机 / 桌面响应式适配
- 滚动错落入场、卡片 3D 倾斜、成长见证卡片切换等轻量动效
- 支持系统「减少动态效果」偏好，开启后自动降级为静态
