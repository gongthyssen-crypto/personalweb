# Thyssen 个人网站

个人主页项目，使用 Flask 提供单页展示。

## 技术栈

- **后端**：Flask
- **前端**：单页 HTML + 内联 CSS（`templates/mainsite.html`）
- **静态资源**：`static/`（头像、背景图等）

## 项目结构

```
personalweb/
├── app.py              # Flask 应用入口，根路由渲染主页
├── templates/
│   └── mainsite.html   # 个人主页模板（关于我、链接等）
├── static/             # 静态文件（需自备 me.png、back.png 等）
│   ├── me.png          # 头像
│   └── back.png        # 首屏背景图
└── README.md
```

## 环境与运行

### 依赖

需要 Python 3 与 Flask：

```bash
pip install flask
```

若使用依赖文件（可选）：

```bash
pip install -r requirements.txt
```

可先创建 `requirements.txt`，内容为：

```
flask>=3.0.0
```

### 启动

在项目根目录执行：

```bash
python app.py
```

默认访问：**http://127.0.0.1:8080**

## 静态资源说明

页面会引用：

- `/static/me.png`：个人头像（建议约 120×120 或正方形）
- `/static/back.png`：首屏背景图（用于 `background-size: cover`，建议横向大图）

请将对应图片放入 `static/` 目录；若目录不存在，可先创建 `static` 文件夹。

## 许可与用途

个人学习与展示用，可按需修改文案与样式。
