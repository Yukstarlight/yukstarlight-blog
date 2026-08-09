# Yukstarlight 博客

个人静态博客 · 部署在 GitHub Pages

## 本地预览

```bash
# 进入目录
cd yukstarlight-blog

# 任选一种方式启动本地服务
python -m http.server 8000
# 或
npx serve .
```

浏览器打开 `http://localhost:8000` 预览。

## 部署到 GitHub Pages

1. 把这个目录 push 到一个 GitHub 仓库（推荐 `Yukstarlight.github.io`）
2. 进入仓库 Settings → Pages
3. Source 选择 `Deploy from a branch`
4. Branch 选择 `main` (或 `master`) + `/ (root)`
5. 保存后等待几分钟，访问 `https://yukstarlight.github.io/`

## 目录结构

```
yukstarlight-blog/
├── index.html              # 博客主页
├── lightsnowtown.html      # 灯雪镇服务器官网
├── lightsnowtown-promo.html # 服务器宣传预览页
├── 赞助图片.jpeg            # 赞助图片
├── server-icon.jpg          # 服务器图标
├── assets/
│   └── avatar.png           # 头像
└── README.md                # 本文件
```

## 自定义

- **个人信息**：直接编辑 `index.html` 顶部的 hero 区
- **社交链接**：编辑 `#socials` section
- **博客文章**：在 `#blog` section 新增 `<a class="blog-card">` 块，或拆分为独立 `posts/` 子目录
- **配色**：修改 `<style>` 里 `:root` 的 CSS 变量

## 技术栈

- 纯 HTML + CSS + JS，无框架依赖
- 自适应移动端
- 星空背景 canvas 动画
- IntersectionObserver 滚动入场
- 液态毛玻璃 / 渐变 / 悬浮动效