# Pixel Reader

单文件、纯前端、离线可用的阅读器。双击 `index.html` 即可使用。

## 功能

- **多格式支持** — EPUB、PDF、DOCX、TXT
- **持久存储** — 书籍数据存入 IndexedDB，关闭浏览器不丢失
- **阅读进度记忆** — 自动保存并恢复上次阅读位置
- **书签系统** — 任意位置添加书签，支持跨书跳转
- **双页模式** — EPUB 下可切换单/双页布局
- **字号调节** — 无级缩放
- **亮度调节** — 暗光环境下降低屏幕亮度
- **位置跳转** — 按页码或百分比快速跳转
- **书架管理** — 搜索、重命名、删除书籍
- **键盘 + 滚轮翻页** — EPUB 滚轮翻页，PDF 滚轮滚动到底自动翻页

## 使用方式

1. 下载 `index.html`
2. 双击在浏览器中打开
3. 点击左侧「书架」按钮，导入书籍
4. 点击书架中的书开始阅读

## 快捷键

| 按键 | 操作 |
|------|------|
| `←` `→` | 翻页 |
| `Esc` | 关闭当前书籍 |

## 技术

纯静态 HTML，使用 CDN 加载以下库：

- [epub.js](https://github.com/futurepress/epub.js) — EPUB 解析与渲染
- [pdf.js](https://github.com/mozilla/pdf.js) — PDF 渲染
- [mammoth.js](https://github.com/mwilliamson/mammoth.js) — DOCX 转 HTML
- [JSZip](https://github.com/Stuk/jszip) — EPUB 解压依赖
