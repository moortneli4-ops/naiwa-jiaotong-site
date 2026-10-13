# 奶娃交通大学.com

访问首页后 **50%** 跳转上海交通大学官网，**50%** 展示 QQ 群拼合图。

## 文件

- `index.html` — 随机分流入口
- `image.html` — 展示拼合图片
- `assets/composite.png` — 两张群邀请图左右拼合

## GitHub Pages 部署

1. 在 GitHub 新建空仓库（建议 `moortneli4-ops/naiwa-jiaotong-site`）
2. 本地推送（需代理时加环境变量）：

```powershell
$env:https_proxy="http://127.0.0.1:7890"
$env:http_proxy="http://127.0.0.1:7890"
$env:GIT_AUTHOR_NAME="Sujun"
$env:GIT_AUTHOR_EMAIL="sujun@users.noreply.github.com"
$env:GIT_COMMITTER_NAME="Sujun"
$env:GIT_COMMITTER_EMAIL="sujun@users.noreply.github.com"
git -C "C:\Users\Sujun\Desktop\sjtu-agent-main\naiwa-jiaotong-site" remote add origin https://github.com/moortneli4-ops/naiwa-jiaotong-site.git
git -C "C:\Users\Sujun\Desktop\sjtu-agent-main\naiwa-jiaotong-site" push -u origin main
```

3. Settings → Pages → `main` / 根目录，保存
4. 域名 DNS（在域名注册商处）：
   - `@` A 记录 → `185.199.108.153`、`185.199.109.153`、`185.199.110.153`、`185.199.111.153`
   - 或 `@` CNAME → `moortneli4-ops.github.io`（部分注册商不支持根域名 CNAME，则用 A 记录）
5. Pages → Custom domain 填 `奶娃交通大学.com`（Punycode: `xn--tlq19wzg6tr9c466m.com`）
6. 勾选 Enforce HTTPS，等待生效

## 本地预览

直接用浏览器打开 `index.html`，多刷新几次可看到两种去向。
