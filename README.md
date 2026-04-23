# 🌐 多语言个人作品集 (中英法三语版)

> **默认语言：** 英语 (English)
> **包含语言：** 英语 (EN), 法语 (FR), 中文 (CN)

---

## 🚀 核心功能特点

1.  **自动默认英文**：刷新页面时，所有内容默认为英文。
2.  **一键切换**：导航栏右上角设有语言切换按钮。
3.  **主题自适应**：
    *   **英语 (EN)**：默认深色风格。
    *   **法语 (FR)**：自动切换深色主题。
    *   **中文 (CN)**：自动切换浅色主题（适合中文阅读）。
4.  **无感体验**：所有文本（导航、标题、描述）实时切换，无需刷新。

---

## 💻 完整网页代码

### 1. HTML 结构 (`index.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <!-- 样式部分放在 CSS 块中 -->
    <style>
        /* --- 基础变量 --- */
        :root {
            --bg-color: #f4f4f4; /* 浅色背景 */
            --text-color: #333;  /* 深色文字 */
            --card-bg: #ffffff;
            --accent-color: #007bff;
            --nav-bg: rgba(255, 255, 255, 0.95);
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
            transition: all 0.3s ease;
        }

        /* --- 语言切换按钮 --- */
        .lang-switcher {
            position: absolute;
            top: 10px;
            right: 10px;
            z-index: 1000;
        }

        .lang-btn {
            background: transparent;
            border: 1px solid #333;
            color: #333;
            padding: 5px 10px;
            cursor: pointer;
            border-radius: 4px;
            font-size: 0.85rem;
            font-weight: bold;
