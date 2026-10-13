# 奶娃交通大学.com

访问首页后 **50%** 跳转上海交通大学官网，**50%** 展示 QQ 群拼合图。

## 文件

- `index.html` — 随机分流入口
- `image.html` — 展示拼合图片
- `assets/composite.png` — 两张群邀请图左右拼合

## GitHub Pages 部署

1. 新建仓库并推送本目录
2. Settings → Pages → 分支 `main` / 根目录
3. 域名 DNS：
   - `@` → GitHub Pages A 记录（185.199.108.153 等四条）
   - 或 CNAME 到 `用户名.github.io`
4. 仓库 Settings → Pages → Custom domain 填 `奶娃交通大学.com`
5. 等待 HTTPS 生效

## 本地预览

直接用浏览器打开 `index.html`，多刷新几次可看到两种去向。
