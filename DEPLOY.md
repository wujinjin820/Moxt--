# Moxt 官网部署指南

## 方式一：Vercel（推荐）

1. **安装 Vercel CLI**（如未安装）：
   ```bash
   npm i -g vercel
   ```

2. **在项目目录执行**：
   ```bash
   cd "/Users/wujinjin/Documents/Moxt 官网 01"
   vercel
   ```

3. 按提示登录、选择项目，即可生成线上地址。

4. **或通过网页部署**：
   - 打开 [vercel.com](https://vercel.com)
   - 导入项目（需先推送到 GitHub）
   - 或直接拖拽项目文件夹到 Vercel 部署

---

## 方式二：Netlify

1. 打开 [netlify.com](https://netlify.com) → **Add new site** → **Deploy manually**
2. 将整个项目文件夹拖入页面
3. 等待部署完成，获得访问链接

---

## 方式三：GitHub Pages

1. 将项目推送到 GitHub 仓库
2. 仓库设置 → **Pages** → Source 选择 **main** 分支
3. 根目录选择 `/ (root)` 或指定包含 `index.html` 的目录
4. 保存后访问 `https://<用户名>.github.io/<仓库名>/`

---

## 部署前检查

确保以下资源存在，否则页面会缺图：

- `assets/images/moxt-logo.svg` - 导航和页脚 Logo
- `assets/images/moxt-logo-mono.svg` - Footer 底部大 Logo
- `assets/images/comp-openclaw.png` - 对比卡片
- `assets/images/comp-chatgpt.png`
- `assets/images/comp-notion.png`
- `assets/images/comp-cursor.png`

当前已有：`hero-workspace.svg`、`sp-context.svg`、`sp-autonomous.svg`、`sp-claws.svg`
