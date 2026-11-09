# 我的博客

GitHub Pages + Jekyll 中文博客。包含响应式首页、文章阅读、分类归档和关于页。

## 首次发布

1. 在 GitHub 新建公开仓库，建议命名为 `你的用户名.github.io`。
2. 上传此目录中的文件（包含 `_layouts`、`_posts`、`assets` 和 `_config.yml`），保留目录结构。
3. 仓库 Settings → Pages → Build and deployment，选择 Deploy from a branch，选择 `main` 和 `/ (root)`，保存。
4. 等待 GitHub 构建成功，访问 `https://你的用户名.github.io`。

如果仓库名称是 `my-blog` 等普通名称，需要将 `_config.yml` 的 `baseurl` 改成 `/my-blog`，访问地址为 `https://你的用户名.github.io/my-blog/`。个人主页仓库的 `baseurl` 保持空字符串。

## 个性化和写作

- `_config.yml`：博客名称和简介；`url` 可填写网站完整域名，不含末尾斜杠。
- `about.md`：个人介绍。
- `_posts/YYYY-MM-DD-slug.md`：文章，文件开头填写 `title` 和 `categories`，参考示例文章。日期不要晚于实际发布日期。
- `assets/style.css`：配色与布局。

在 GitHub 编辑或添加文章并提交后，Pages 会重新构建。网站不需要放置 GitHub Token。

## 本地预览（可选）

安装 Ruby 和 Bundler 后，运行 `bundle install`，然后运行 `bundle exec jekyll serve`，打开输出的本地地址。

GitHub Pages 托管静态网站，不运行自定义服务端程序。此版本通过 GitHub 网页或本地 Markdown 编辑文章，没有访客登录、在线编辑后台或数据库。
