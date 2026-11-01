# Guoxu Zhao 的博客

这个静态博客由 GitHub Pages 和 Jekyll 构建，不需要租服务器、配置数据库或运行 Django。

## 修改个人信息

- 修改 `_config.yml` 中的 `title` 和 `description`，调整网站名称和简介。
- 修改 `about.md`，填写个人介绍和希望公开的联系方式。
- 修改 `_layouts/default.html` 中的导航或 GitHub 链接。
- 修改 `assets/blog.css`，调整颜色、字体和排版。

## 写文章

1. 参考 `_drafts/my-first-post.md`，新建一个 Markdown 文件，放在 `_posts` 文件夹中。
2. 文件名必须是 `年-月-日-英文标题.md`，例如 `2026-11-01-my-first-post.md`。
3. 文件开头保留以下内容，然后在下面写文章：

   ```markdown
   ---
   layout: post
   title: 文章标题
   ---

   这里是文章内容，支持 Markdown。
   ```

4. 保存后提交并推送。GitHub Pages 构建成功后，文章会自动出现在首页。默认不显示未来日期的文章。

## 上传修改

```bash
cd /Users/zguoxu/Desktop/blog
git add .
git commit -m "更新博客"
git push
```

首次配置 GitHub Pages：进入仓库 Settings → Pages，在 Build and deployment 下选择 Deploy from a branch，选择 `main` 和 `/ (root)`，保存。状态可在仓库的 Actions 页面查看。

本地原 DjangoBlog 源码为了参考而保留，不会随静态博客上传。静态站没有 Django 后台；文章通过 Markdown 文件维护。不要把密码或私人资料放进这个公开仓库。
