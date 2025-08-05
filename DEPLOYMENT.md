# GitHub Pages 部署指南

## 快速部署步骤

### 1. 创建GitHub仓库
- 登录GitHub
- 点击 "New repository"
- 仓库名建议使用 `yourusername.github.io` (个人主页) 或任意名称
- 设置为Public
- 不要初始化README (因为我们已经有了)

### 2. 上传代码
有几种方式：

#### 方式A: 通过GitHub网页界面
1. 在新创建的仓库页面点击 "uploading an existing file"
2. 拖拽或选择所有文件 (`index.html`, `README.md`, `_config.yml`)
3. 写提交信息: "Initial commit - Academic homepage"
4. 点击 "Commit changes"

#### 方式B: 通过Git命令行
```bash
# 在项目文件夹中初始化git
git init

# 添加远程仓库
git remote add origin https://github.com/yourusername/yourrepository.git

# 添加所有文件
git add .

# 提交
git commit -m "Initial commit - Academic homepage"

# 推送到GitHub
git push -u origin main
```

### 3. 启用GitHub Pages
1. 进入仓库的 Settings 页面
2. 滚动到 "Pages" 部分
3. 在 "Source" 下选择 "Deploy from a branch"
4. 选择 "main" 分支
5. 选择 "/ (root)" 文件夹
6. 点击 "Save"

### 4. 访问网站
- 等待几分钟让GitHub处理
- 网站地址通常是: `https://yourusername.github.io/repository-name`
- 如果仓库名是 `yourusername.github.io`，地址就是: `https://yourusername.github.io`

## 更新网站内容

### 添加新论文
1. 编辑 `index.html`
2. 在 "Working Papers" 部分添加新的论文块
3. 提交并推送更改

### 更新个人信息
1. 修改联系信息、教育背景等
2. 更新 Work in Progress 列表
3. 提交更改

### 添加图片或文档
1. 创建 `assets` 文件夹
2. 上传图片或PDF文件
3. 在HTML中引用: `<img src="assets/photo.jpg" alt="Photo">`

## 故障排除

### 网站没有显示更新
- 等待5-10分钟让GitHub处理
- 检查仓库的 Actions 页面是否有错误
- 清除浏览器缓存

### 样式显示不正确
- 确保 `index.html` 中的CSS没有被修改破坏
- 检查文件编码是否为UTF-8

### 联系链接不工作
- 更新 `index.html` 中的链接地址
- 移除 `onclick="alert(...)"` 并替换为实际链接

## 高级定制

### 添加谷歌分析
在 `<head>` 部分添加GA代码

### 自定义域名
1. 在仓库根目录创建 `CNAME` 文件
2. 文件内容为你的域名: `www.yourdomain.com`
3. 在域名提供商处设置DNS指向GitHub Pages

### 添加更多页面
1. 创建新的HTML文件 (如 `publications.html`)
2. 在导航中添加链接
3. 保持统一的样式

---

**提示**: 第一次部署可能需要等待几分钟。之后的更新通常会在1-2分钟内生效。
