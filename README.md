# 酒店民宿长图编辑器

零构建、无后端依赖的静态网页工具，用于制作酒店和民宿宣传长图。

## 本地运行

```bash
python3 -m http.server 4321
```

打开 `http://localhost:4321/index.html`。

## 发布方式

### GitHub Pages

1. 创建一个空 GitHub 仓库。
2. 将本目录推送到仓库的 `main` 分支。
3. 在仓库 Settings > Pages 中选择 GitHub Actions。
4. `.github/workflows/pages.yml` 会自动发布网站。

### Vercel

将本目录导入 Vercel，无需构建命令，输出目录使用项目根目录。

### Netlify

将本目录拖入 Netlify Drop，或连接 Git 仓库。`netlify.toml` 已配置发布目录。

## 数据说明

- 普通保存使用当前浏览器的本地存储，不会上传图片或项目内容。
- “导出项目文件”会生成包含文字、布局和图片的 JSON 文件。
- 其他用户导入该 JSON 文件后可以继续编辑。
- 工具部署后，“复制工具链接”可以分享网页地址，但不会把当前项目数据附加到链接。
