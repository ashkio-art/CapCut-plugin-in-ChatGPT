# GitHub Pages 部署说明

这份文件是独立的 GitHub Pages 备用站部署包。现有 chatgpt.site 和 Netlify 网站不受影响。

## 1. 解压
解压 GitHub-Pages-Deployment.zip。index.html、style.css、app.js、assets 文件夹应在同一层。

## 2. 新建仓库并上传
登录 https://github.com ，新建仓库，建议名为 capcut-guide。
使用 GitHub Free 时，仓库选择 Public。上传后的网页文件及素材也会公开。
在仓库选择 Add file > Upload files。
上传解压后的所有文件和 assets 文件夹，然后点击 Commit changes。
请上传解压后的内容，不要直接上传 zip，也不要把外层文件夹一起上传。
在仓库首页应直接看到 index.html，assets 内应有图片、Logo 和 final-video.mp4。

.nojekyll 是一个空文件，用来跳过默认的 Jekyll 处理。若上传时没带上，可在仓库中选择 Add file > Create new file，命名为 .nojekyll 并提交。

## 3. 开启 Pages
仓库顶部 Settings > 左侧 Pages。
Build and deployment > Source 选择 Deploy from a branch。
Branch 选择 main，文件夹选择 / (root)，点击 Save。
若默认分支名称不是 main，选择实际上传文件的分支。
等待发布完成，然后回到此页点击 Visit site。发布可能需要约 10 分钟。
通常网址为 https://你的用户名.github.io/capcut-guide/ ，以后台实际显示的链接为准。

## 4. 检查
查看首页、Logo 和两张角色图片；点击图片放大；复制两段 prompt；播放视频并检查声音和进度条；点击 CapCut 按钮确认跳转。
资源均使用相对路径，支持仓库名称形成的子目录网址。
无需构建命令、API Key 或环境变量。

## 5. 后续更新
修改后上传同名文件并提交，Pages 会重新发布。原 chatgpt.site、Netlify 与 GitHub Pages 需分别更新。
部署成功后，关闭电脑或删除本地解压文件不会影响线上版本，但建议保存压缩包备份。

官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
