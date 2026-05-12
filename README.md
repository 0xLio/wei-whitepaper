# WEI Web

静态站点：首页为 WEI 数据看板（演示数据 + 图表），**白皮书**为独立页面，可从首页「白皮书 / Whitepaper」进入。

## 本地预览

```bash
python3 -m http.server 8080
```

浏览器打开 `http://localhost:8080`（首页），`http://localhost:8080/whitepaper.html`（白皮书）。

## 部署到 Vercel

根目录含 `index.html` 即可；**Framework Preset** 选 **Other**，无需构建命令。

## 文件说明

| 文件 | 说明 |
| ---- | ---- |
| `index.html` | 首页看板（链上交互为演示 UI） |
| `whitepaper.html` | 白皮书（中英文，与上游 `wei-whitepaper.html` 同步） |

## 与仓库外源文件同步

若在 `Paper/wei-whitepaper.html` 编辑白皮书：

```bash
cp ../wei-whitepaper.html ./whitepaper.html
```
