# 添加头像图片说明

## 头像文件要求

您需要将学术头像文件命名为：`eb8a0749e8890937cddfd361c55d85e.jpg`

## 放置位置

将头像文件放在与 `index.html` 相同的文件夹中：

```
项目文件夹/
├── index.html
├── eb8a0749e8890937cddfd361c55d85e.jpg  ← 头像文件
├── README.md
└── _config.yml
```

## 图片建议

- **尺寸：** 建议 400x400 像素或更高分辨率的正方形图片
- **格式：** JPG 或 PNG 都可以
- **大小：** 建议小于 500KB 以确保快速加载
- **内容：** 专业的学术照片，背景简洁

## 如果要更改头像文件名

如果您想使用不同的文件名，需要在 `index.html` 中修改这一行：

```html
<img src="您的头像文件名.jpg" alt="Mingyu Shu" class="profile-photo">
```

## 在 GitHub Pages 上部署

当您将代码上传到 GitHub 时，确保头像文件也一起上传。头像会显示在网站的右上角。
