# 星擎 Landing Page

AI驱动的视频创作平台官网

## 📁 项目结构

```
.
├── index.html          # 主页面
├── images/            # 图片资源
│   ├── dashboard.png  # 数据看板截图
│   ├── compose.png    # 视频合成截图
│   ├── publish.png    # 发布截图
│   └── slice.png      # 视频切片截图
└── README.md          # 本文件
```

## 🚀 本地预览

### 方法一：使用 Python
```bash
python3 -m http.server 8080
```
然后访问：http://localhost:8080/index.html

### 方法二：使用 Node.js
```bash
npx serve .
```

### 方法三：直接打开
在浏览器中打开 `file:///完整路径/index.html`

## 📦 技术栈

- **HTML5** - 语义化标签
- **Tailwind CSS** - 通过 CDN 引入（无需安装）
- **原生 JavaScript** - 动画和交互效果
- **纯静态** - 无需后端，可直接部署

## 🎨 特性

- ✅ 响应式设计（支持桌面/平板/手机）
- ✅ 流畅动画效果（滚动触发、数字翻滚）
- ✅ 渐变色主题（紫蓝色系）
- ✅ 深色模式风格
- ✅ 交互式工作流展示
- ✅ 动态背景效果

## 🌐 部署方式

### Vercel 部署
```bash
# 1. 安装 Vercel CLI
npm i -g vercel

# 2. 在项目目录运行
vercel

# 3. 按提示完成部署
```

### Netlify 部署
1. 登录 Netlify
2. 拖拽整个文件夹到 Netlify
3. 自动部署完成

### GitHub Pages 部署
```bash
# 1. 初始化 git 仓库
git init
git add .
git commit -m "Initial commit"

# 2. 创建 GitHub 仓库并推送
git remote add origin <your-repo-url>
git branch -M main
git push -u origin main

# 3. 在 GitHub 仓库设置中启用 Pages
Settings → Pages → Source: main branch
```

### 传统服务器部署
将所有文件上传到服务器的 web 根目录（如 `/var/www/html/`）

## 🔧 注意事项

### 外部依赖
- **Tailwind CSS**：通过 CDN 加载，需要网络连接
- **Figma 图片**：部分图标使用 Figma API，建议替换为本地资源

### 图片优化建议
当前 images/ 文件夹共 7.4MB，建议：
- 使用 TinyPNG 压缩图片（可减少 50-70% 体积）
- 考虑使用 WebP 格式（更小更快）
- 启用 CDN 加速图片加载

### 字体
页面使用 Google Fonts：
- **Inter** - 主字体
- **Noto Sans SC** - 中文字体
- **DIN Alternate** - 数字字体

## 📱 浏览器兼容性

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

## 🎯 性能优化建议

1. **图片懒加载**：可添加 `loading="lazy"` 属性
2. **Tailwind 优化**：生产环境使用 PurgeCSS 移除未使用的样式
3. **压缩代码**：使用工具压缩 HTML/CSS/JS
4. **CDN 加速**：将静态资源托管到 CDN

## 📞 技术支持

如有问题，请联系开发团队。

---

**最后更新**：2026-03-25
**版本**：1.0.0
