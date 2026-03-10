# 部署获取外部链接

## 方式 A：Netlify 拖拽部署（最快，无需 Git）

1. 打开 [app.netlify.com/drop](https://app.netlify.com/drop)
2. 将整个项目文件夹 `Moxt 官网 00` 拖入页面
3. 等待几秒，即可获得一个随机链接（如 `https://xxx.netlify.app`）
4. 无需登录、无需 GitHub

---

## 方式 B：GitHub Pages

### 步骤 1：在 GitHub 创建仓库

1. 打开 [github.com/new](https://github.com/new)
2. 仓库名填写：`moxt-website`（或任意名称）
3. 选择 **Public**
4. **不要**勾选 "Add a README file"
5. 点击 **Create repository**

## 步骤 2：推送代码

在终端执行（将 `YOUR_USERNAME` 替换为你的 GitHub 用户名）：

```bash
cd "/Users/wujinjin/Documents/Moxt 官网 00"

git remote add origin https://github.com/YOUR_USERNAME/moxt-website.git
git branch -M main
git push -u origin main
```

## 步骤 3：开启 GitHub Pages

1. 进入仓库页面 → **Settings** → 左侧 **Pages**
2. **Source** 选择 **Deploy from a branch**
3. **Branch** 选择 `main`，文件夹选 `/ (root)`
4. 点击 **Save**

## 步骤 4：获取链接

等待 1–2 分钟部署完成后，访问：

```
https://YOUR_USERNAME.github.io/moxt-website/
```

---

**备选：Vercel 部署（更快）**

1. 打开 [vercel.com](https://vercel.com) 并登录
2. **Add New** → **Project** → 选择 **Import Git Repository**
3. 先完成上述步骤 1、2 推送代码到 GitHub
4. 在 Vercel 中导入该仓库，直接部署
5. 会得到类似 `https://moxt-website-xxx.vercel.app` 的链接

---

## 打不开？常见问题

**GitHub Pages 404：**
- 确认链接格式：`https://用户名.github.io/仓库名/`（末尾斜杠要有）
- 仓库必须是 **Public**
- Settings → Pages 里 Source 选 `main`，文件夹选 `/(root)`
- 首次部署需等待 2–5 分钟

**资源加载失败：**
- 检查是否推送到 `main` 分支
- 确认 `index.html` 在仓库根目录
