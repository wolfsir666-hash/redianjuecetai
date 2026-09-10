# 社媒热点决策台

一个纯静态的内容电商「热点 → 决策」看板，聚合 Amazon 商品数据、TikTok 热点话题、达人与爆款视频样本，按优先级输出热点货盘与行动建议。

## 部署到 GitHub Pages

1. 新建一个 GitHub 仓库（例如 `hotspot-desk`）。
2. 把本目录下的所有文件（含 `index.html`、`img/`、`vimg/`、`.nojekyll`）全部推到仓库的 `main` 分支根目录：
   ```bash
   git init
   git add -A
   git commit -m "社媒热点决策台"
   git branch -M main
   git remote add origin https://github.com/<你的用户名>/<仓库名>.git
   git push -u origin main
   ```
3. 打开仓库 **Settings → Pages**，Source 选 `Deploy from a branch`，Branch 选 `main` / `/(root)`，保存。
4. 等一两分钟，访问 `https://<你的用户名>.github.io/<仓库名>/` 即可。

## 说明

- 纯静态页面，无需任何后端或构建步骤，浏览器直接打开 `index.html` 也能看。
- `.nojekyll` 用于关闭 GitHub Pages 的 Jekyll 处理，避免个别资源被忽略。
- 所有图片为本地相对路径（`img/`、`vimg/`），已随包提供。
