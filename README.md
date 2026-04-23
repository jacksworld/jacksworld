# 个人主页 | 简历模板

这是一份包含完整 HTML 结构、CSS 样式和 JavaScript 交互功能的个人主页代码。您可以将其保存为 `index.html` 并在浏览器中直接查看效果。

## 📄 完整代码

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我的个人主页</title>
    <style>
        /* 基础样式 */
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; line-height: 1.6; color: #333; }
        .container { max-width: 1100px; margin: 0 auto; padding: 0 20px; }
        
        /* 导航栏 */
        nav { display: flex; justify-content: space-between; align-items: center; padding: 20px 0; }
        .logo { font-size: 24px; font-weight: bold; color: #222; }
        .nav-links { list-style: none; display: flex; gap: 20px; }
        .nav-links a { text-decoration: none; color: #333; transition: 0.3s; }
        .nav-links a:hover { color: #007bff; }
        .menu-toggle { display: none; font-size: 24px; cursor: pointer; }
        
        /* Hero 区域 */
        .hero { height: 80vh; display: flex; align-items: center; justify-content: center; text-align: center; background: #f4f4f4; }
        .hero h1 { font-size: 48px; margin: 10px 0; }
        .hero h2 { font-size: 24px; color: #666; }
        .btn { padding: 10px 20px; background: #007bff; color: white; text-decoration: none; border-radius: 5px; }

        /* 通用样式 */
        section { padding: 60px 0; }
        .section-title { text-align: center; font-size: 32px; margin-bottom: 40px; }

        /* 关于我 */
        .about-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; }
        .skills ul { list-style: none; }
        .skills li { margin-bottom: 10px; padding-left: 20px; border-left: 3px solid #007bff; }

        /* 经历时间线 */
        .timeline { max-width: 800px; margin: 0 auto; }
        .card { border: 1px solid #ddd; padding: 20px; border-radius: 8px; margin-bottom: 20px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
        .date { color: #999; font-size: 14px; display: block; margin-bottom: 10px; }

        /* 页脚 */
        footer { background: #222; color: white; padding: 40px 0; text-align: center; }
        footer p { margin: 5px 0; }

        /* 响应式适配 */
        @media (max-width: 768px) {
            .nav-links { display: none; }
            .menu-toggle { display: block; }
            .about-grid { grid-template-columns: 1fr;
