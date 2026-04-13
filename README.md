# 蛤蛤体生成器

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen)](https://wenyinos.github.io/haha/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-brightgreen)](https://getbootstrap.com)

在线演示：https://WenYin-Community.github.io/haha/

## 简介

模仿*******说话风格的文本生成器。根据填入的关键词自动生成一段"蛤蛤体"风格的对话。

## 功能

### 核心功能
- **个性化生成**：填写13个自定义关键词，生成独一无二的蛤蛤体文本
- **随机初始化**：页面加载时自动随机填充示例数据，方便快速预览
- **实时预览**：点击"生成"按钮即时查看结果

### 可自定义的关键词
| 序号 | 字段 | 说明 | 示例值 |
|:---:|:---|:---|:---|
| 1 | 标题来源 | 说话者身份 | **** |
| 2 | 标题去向 | 说话对象 | 香港记者 |
| 3-13 | 正文内容 | 事件、人物、地点等 | 详见页面表单 |

### 技术特性
- 响应式设计，适配桌面端和移动端
- 采用 Bootstrap 5 框架
- 纯前端实现，无需后端服务
- 预置默认示例数据，开箱即用

## 技术栈

- HTML5
- CSS3
- JavaScript (原生)
- [Bootstrap 5](https://getbootstrap.com)

## 项目结构

```
haha/
├── index.html          # 主页面
├── images/
│   ├── favicon.ico     # 网站图标
│   └── favicon.png    # PNG 图标
├── stylesheets/       # 原始样式文件（保留）
└── javascripts/       # 原始脚本文件（保留）
```

## 本地运行

```bash
# 克隆仓库
git clone https://github.com/wenyinos/haha.git
cd haha

# 使用静态服务器打开 index.html
# 方式一：Python
python -m http.server 8080

# 方式二：PHP
php -S localhost:8080

# 方式三：Node.js
npx http-server -p 8080
```

访问 http://localhost:8080 即可使用。

## 开发指南

### 修改模板文本
编辑 `index.html` 中的 `template` 变量（第282-311行）来自定义生成文本的模板。

### 添加新的关键词
1. 在表单中添加新的 `<input>` 元素
2. 在 `init_arrays` 中添加对应的默认值
3. 在 `template` 中使用 `{{字段名}}` 占位符

### 样式调整
- 修改 `<style>` 标签中的 CSS 自定义样式
- 或覆盖 Bootstrap 默认样式

## 灵感来源

- 原版作者：[dkwingsmt/haha](https://github.com/dkwingsmt/haha)
- 参考人物：[张成愈](http://photo.renren.com/photo/302760940/photo-7757506381)

## 更新日志

### v2.0.0 (2026-04-10)
- 使用 Bootstrap 5 重构 UI
- 响应式布局优化
- 添加自定义 favicon
- 重写 README.md 文档

### v1.0.0
- 初始版本
- 基础蛤蛤体生成功能

## License

Public Domain

---

Made with ❤️ by [wenyinos](https://github.com/wenyinos)
