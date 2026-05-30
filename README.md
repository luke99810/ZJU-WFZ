# 学术个人主页使用指南

## 文件结构

```
.
├── index.html      # 主页面（修改个人信息）
├── style.css       # 样式文件（一般不需要改）
├── photo.jpg       # 个人照片（需自行添加）
├── cv-cn.pdf       # 中文简历（需自行添加）
├── cv-en.pdf       # 英文简历（需自行添加）
└── README.md       # 本说明文件
```

## 快速开始

### 1. 修改个人信息

打开 `index.html`，替换以下内容：

- **姓名**：搜索 `你的名字` 和 `Your Name` 进行替换
- **学校/学院**：修改所在大学、学院信息
- **联系方式**：邮箱、电话/微信
- **研究兴趣**：修改为你的研究方向
- **论文列表**：添加你的论文信息
- **项目经历**：添加你的科研项目
- **教育经历**：修改你的学历背景
- **荣誉奖项**：添加你的获奖记录

### 2. 添加个人照片

将你的证件照命名为 `photo.jpg`，放在同一目录下。建议尺寸：宽 180px，高 240px。

### 3. 添加简历文件

- 中文简历命名为 `cv-cn.pdf`
- 英文简历命名为 `cv-en.pdf`

### 4. 本地预览

直接用浏览器打开 `index.html` 即可预览效果。

## 部署到 GitHub Pages（免费）

### 步骤 1：创建 GitHub 账号
访问 https://github.com 注册账号。

### 步骤 2：创建仓库
1. 点击右上角 `+` → `New repository`
2. 仓库名填写：`你的用户名.github.io`
   - 例如：用户名为 `john`，则填写 `john.github.io`
3. 选择 `Public`（公开）
4. 点击 `Create repository`

### 步骤 3：上传文件
1. 进入刚创建的仓库
2. 点击 `Add file` → `Upload files`
3. 上传以下文件：
   - `index.html`
   - `style.css`
   - `photo.jpg`（你的照片）
   - `cv-cn.pdf`（中文简历）
   - `cv-en.pdf`（英文简历）
4. 点击 `Commit changes`

### 步骤 4：开启 GitHub Pages
1. 进入仓库的 `Settings`（设置）
2. 左侧菜单点击 `Pages`
3. Source 选择 `Deploy from a branch`
4. Branch 选择 `main`，文件夹选择 `/ (root)`
5. 点击 `Save`

### 步骤 5：访问网站
等待 1-2 分钟后，访问：
```
https://你的用户名.github.io
```

## 后续更新

需要更新内容时：
1. 修改 `index.html` 中的内容
2. 重新上传到 GitHub 仓库
3. 等待自动部署（约 1-2 分钟）

## 自定义建议

### 修改配色
编辑 `style.css` 中的 `:root` 部分：
```css
:root {
    --primary-color: #2c3e50;  /* 主色调 */
    --accent-color: #3498db;   /* 强调色（链接颜色） */
    /* ... */
}
```

### 添加 Google Scholar 链接
在导航栏中找到：
```html
<li><a href="https://scholar.google.com" target="_blank">Google Scholar</a></li>
```
将链接替换为你的真实 Google Scholar 主页地址。

### 添加 GitHub 链接
```html
<li><a href="https://github.com/你的用户名" target="_blank">GitHub</a></li>
```

## 常见问题

**Q: 照片不显示？**
A: 确保照片命名为 `photo.jpg`，且与 `index.html` 在同一目录。

**Q: 如何添加更多论文？**
A: 复制 `.paper-item` 区块，粘贴到论文列表中即可。

**Q: 手机上看样式错乱？**
A: 已内置响应式设计，确保 `style.css` 正确上传。

**Q: 如何绑定自定义域名？**
A: 在仓库设置中添加 `CNAME` 文件，内容为你的域名（如 `www.yourname.com`），然后在域名服务商处添加 CNAME 记录指向 `你的用户名.github.io`。

## 技术支持

如有问题，可以：
1. 查看 GitHub Pages 官方文档：https://pages.github.com/
2. 搜索相关教程
3. 咨询有经验的同学或老师

