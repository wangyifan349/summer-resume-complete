# Summer Resume ☀️

Summer Resume 是一个基于 Bootstrap 5 构建的响应式个人简历与 GitHub 作品集静态网站。页面采用橘红色夏日主题，以真实开源项目为核心内容，用于展示项目用途、实现范围、技术能力、教育背景、求职意向与联系方式。

当前版本已配置为王一帆的个人简历，可直接部署到 GitHub Pages。项目不需要安装依赖或执行构建命令，上传文件后即可作为静态网站运行。

## ✨ 页面内容

- **代表性开源项目**：优先展示云盘、代理工具、密码与安全笔记、业务后端、人脸检索、加密通信和 Rust 网络代理等项目。
- **项目说明**：每个项目包含用途、主要功能、实现范围、技术标签及 GitHub 仓库链接。
- **求职意向**：说明 Python、Rust、后端开发、Linux 服务端、网络编程和模型部署等岗位方向。
- **技术能力**：介绍 Python、Flask、FastAPI、Rust、计算机视觉、向量检索、网络协议、加密软件和 Linux 部署能力。
- **个人信息**：包含教育背景、邮箱、电话和 GitHub 主页。
- **交互功能**：支持手机与电脑布局、移动端导航、深浅色模式、锚点定位、折叠内容以及打印或保存 PDF。

## 🧰 代表性 GitHub 项目

- `github.com/wangyifan349/single-file-flask-drive`
- `github.com/wangyifan349/AegisRoute`
- `github.com/wangyifan349/CipherNoteVault`
- `github.com/wangyifan349/provincial-government-service-platform`
- `github.com/wangyifan349/face-search-tools`
- `github.com/wangyifan349/xfm4-secure-mux`
- `github.com/wangyifan349/rproxy`

## 📁 发布版文件结构

```text
summer-resume-release/
├── index.html           # 中文首页
├── index-en.html        # 英文页面
├── hero-summer.webp     # 首页背景
├── summer-texture.webp  # 页面内容背景
├── github-summer.webp   # 项目展示区背景
└── README.md            # 项目说明
```

页面样式和交互脚本已经写入两个 HTML 文件。图片为独立 WebP 文件，没有使用 Base64 或 Data URI 编码。

## 🧱 项目性质

本项目是**纯静态网站**，不包含后端服务、数据库、登录系统、在线表单处理或内容管理后台。

- 邮件按钮使用 `mailto:` 链接。
- 电话按钮使用 `tel:` 链接。
- 项目按钮直接跳转到公开 GitHub 仓库。
- Bootstrap CSS 与 JavaScript 通过 CDN 加载，因此首次访问需要能够连接 CDN。

## 🚀 本地查看

可以直接双击 `index.html`。为获得更稳定的本地预览效果，也可以在项目目录运行：

```bash
python -m http.server 8000
```

然后访问：

```text
http://127.0.0.1:8000/
```

英文页面：

```text
http://127.0.0.1:8000/index-en.html
```

## 🌐 部署到 GitHub Pages

1. 将本目录中的 6 个文件上传到 GitHub 仓库根目录。
2. 打开仓库的 **Settings → Pages**。
3. 在 **Build and deployment** 中选择 **Deploy from a branch**。
4. Branch 选择 `main`，Folder 选择 `/ (root)`。
5. 点击 **Save**，等待 GitHub 完成发布。

默认中文页面：

```text
https://wangyifan349.github.io/summer-resume-complete/
```

英文页面：

```text
https://wangyifan349.github.io/summer-resume-complete/index-en.html
```

GitHub Pages 会自动加载根目录中的 `index.html`。以后更新文件并提交到 `main` 分支，网站会自动重新发布。

## ⚙️ 修改个人资料

中文和英文内容分别位于：

```text
index.html
index-en.html
```

可以在代码编辑器中搜索以下内容进行替换：

```text
王一帆
wangyifangwbk@163.com
0631-15634319945
wangyifan349
青岛工学院
```

修改项目卡片时，建议同时更新：

- 项目名称；
- 项目介绍；
- 技术标签；
- GitHub 链接的 `href`；
- 页面中显示的仓库路径。

不同语言页面是两个独立 HTML 文件。修改个人信息或项目内容后，应同步更新对应页面。

## 🖼️ 替换背景图片

可直接使用新的 WebP 图片覆盖以下文件，并保持文件名不变：

```text
hero-summer.webp
summer-texture.webp
github-summer.webp
```

建议首页和项目区背景使用接近 `16:9` 的横向图片，内容背景使用较轻的纹理或渐变，避免影响文字可读性。
