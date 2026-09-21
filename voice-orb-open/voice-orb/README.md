# VOICE ORB · 余音栖于此处

一个纯静态的**音频可视化**单页 —— 一颗会呼吸的球，跟着声音的形状变化。

导入一段音频，或者让它听周围的环境声，球都会跟着动。

没有服务端、没有账号、没有联网请求。全部使用浏览器原生 Web API，不向任何服务器发送数据。

![无依赖](https://img.shields.io/badge/dependencies-0-brightgreen) ![单文件](https://img.shields.io/badge/single--file-yes-blue)

---

## 两种输入

| 输入 | 说明 | 本地可用 |
|---|---|---|
| **麦克风** | 球的形态跟着环境声音实时变化 | ❌ 需 HTTPS |
| **音频** | 选择本地音频文件播放，球跟着音乐变化 | ✅ |

右上角 **⚙** 可以调：球体尺寸、模糊强度、呼吸幅度、音频灵敏度、光晕扩散、信号阻尼。

---

## 怎么用

### 方式一：直接打开（部分功能受限）

双击 `index.html` 即可，**音频**模式能正常使用。

但**麦克风不能用** —— 浏览器规定 `getUserMedia` 必须在 HTTPS 环境下才允许调用。这是浏览器的安全策略，不是页面的问题。

### 方式二：部署到静态托管（推荐）

扔到任何静态托管上，就会自动获得 HTTPS，麦克风随之可用：

- **Netlify Drop** — 打开 `app.netlify.com/drop`，把文件夹拖进去，立刻给你一个网址，不用注册也能先试
- **Vercel** — 拖文件夹上传，得到 `xxx.vercel.app`
- **GitHub Pages** — 推到仓库，开启 Pages
- **Cloudflare Pages** — 同理

> ⚠️ GitHub Pages 和 Vercel 在中国大陆访问可能较慢或不稳定。

---

## 隐私

不采集、不上传、不联网。所有音频都在你自己的浏览器里解析，关掉页面就没了。

---

## 许可

**PolyForm Noncommercial 1.0.0** —— 个人使用、学习、研究、自娱自乐，随便用随便改。

**不允许商用。** 想拿去卖钱、或者放进商业产品里，请先联系我。

---

Made for anyone who wants a small quiet thing that breathes.
