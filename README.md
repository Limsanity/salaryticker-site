# 支持 / 隐私政策静态页

App Store Connect 要填两个网址（必填）：

- **支持网址** → `https://<你的域名或 Pages 地址>/`
- **隐私政策网址** → `https://<你的域名或 Pages 地址>/privacy.html`

这两个文件就是给它们用的，纯静态、无依赖，放哪都行。

## 已发布 ✅

- 仓库：<https://github.com/Limsanity/salaryticker-site>
- 支持网址：<https://limsanity.github.io/salaryticker-site/>
- 隐私政策网址：<https://limsanity.github.io/salaryticker-site/privacy.html>

改完内容后：

```bash
cd AppStore/site
git add -A && git commit -m "update pages" && git push
```

Pages 会自动重新构建（约 1 分钟）。

## 其他方案

- Cloudflare Pages / Vercel / Netlify：把 `AppStore/site` 目录拖进去，秒出域名。
- 已有博客：把 `index.html`、`privacy.html`、`icon.png`、`hero.png` 四个文件丢到任意静态目录即可。

## 改内容

- 联系方式目前指向 GitHub Issues，想换成邮箱就全局替换 `github.com/Limsanity/salaryticker-site/issues`。
- 「最后更新」日期记得跟着改。
- 如果以后加了联网功能（比如同步、崩溃统计），这个页面的「不联网、不收集」必须同步改，否则会被审核打回。
