# WEI Whitepaper

静态单页：WEI 项目白皮书（中英文切换），可直接部署到 Vercel。

## 本地预览

在项目根目录执行：

```bash
python3 -m http.server 8080
```

浏览器打开 `http://localhost:8080`。

## 部署到 Vercel（连接 GitHub）

1. 将本仓库推送到 GitHub（若尚未推送，见下方「首次推送」）。
2. 打开 [Vercel](https://vercel.com)，使用 GitHub 账号登录。
3. **Add New… → Project**，选择该仓库。
4. **Framework Preset** 选 **Other**（或 “Other”），无需构建命令；**Root Directory** 保持仓库根目录（本仓库根目录即包含 `index.html`）。
5. 点击 **Deploy**。完成后会得到类似 `https://<项目名>.vercel.app` 的地址。

无需额外配置：`index.html` 位于仓库根目录时，Vercel 会作为静态站点托管。

### 使用 Vercel CLI（可选）

```bash
npm i -g vercel
cd wei-whitepaper-web
vercel
```

按提示登录并关联项目即可。

## 文件说明

| 文件        | 说明           |
| ----------- | -------------- |
| `index.html` | 白皮书完整页面 |
