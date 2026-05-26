# AnyJob 网站复刻

复刻自 `https://talent.anyhelper.net`（AnyJob —— 新一代 AI 驱动的人才引擎）。

## 内容

- `index.html` —— 站点入口，跳转到登录页（对应原站 `/` → `login.php` 的行为）
- `login.html` —— 登录页（公开页面）的忠实静态复刻
- `assets/` —— 图片与第三方脚本（lucide、jQuery、CryptoJS/sha512）
- `ASLibrary/` —— 站点自有脚本（asengine、login、register）

## 说明

- 这是**前端静态复刻**。登录表单会把 SHA512 加密后的密码 POST 到 `ASEngine/ASAjax.php`，
  该后端接口不在本仓库内，因此静态环境下登录不会真正生效。
- 本地预览：在仓库根目录执行 `python3 -m http.server 8000`，浏览器打开 `http://localhost:8000`。
