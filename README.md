# Codex 账号格式转换器（Render 静态部署版）

这是一个纯静态网页，适合直接部署到 Render Static Site。

## 文件说明

- `index.html`：转换器页面，支持粘贴/上传标准 TXT(JSONL)，并导出 Sub2API JSON / CPA tar。
- `render.yaml`：Render Blueprint 配置。

## Render 部署方式

1. 新建一个 GitHub 仓库，只上传本目录里的文件。
2. Render 选择 `New +` -> `Blueprint`，连接该 GitHub 仓库。
3. Render 会读取 `render.yaml` 并创建静态站点。

如果不用 Blueprint，也可以选择 `New +` -> `Static Site`：

- Build Command：留空
- Publish Directory：`.`

## 注意

网页在浏览器本地转换，不需要后端，不会主动上传账号数据。
