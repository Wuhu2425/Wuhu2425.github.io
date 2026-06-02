### 前言
先聊一聊利用Gmeek在github中创建自己的博客的优缺点；
下面是它的优势：
1. 简单且轻量，界面简洁清爽，无需编程基础；
2. 基于Github Issues写作，支持MarkDown，可以随时修改，回溯；
3. 生成基于Github Issues的评论区，访客用GitHub账号即可留言；
4. 正文在Github Issues上，对搜索引擎爬虫友好，被搜索到的概率相比传统静态博客有一定优势。

接下来说说它的缺点：
1. 定制灵活性低；
2. 国内访问速度和稳定性低；
3. 与主流博客框架项目有差距，主题生态，插件支持，社区规模尚显不足。
4. 空间容量有限，1Gb可能对于有重度需求的人略显不足

总结：适合对于追求内容创作，对界面和功能要求不高的纯写作者。
----
### 接下来介绍如何利用Gmeek在github创建自己的blog
#### 1. 创建仓库
访问https://github.com/Meekdai/Gmeek ，下滑在README板块中，点击 _通过模板创建仓库_ 进入创建仓库页面；在 _Repository name_ 输入栏，输入`xxx.github.io`（xxx建议为你的github用户名），然后点击 _create repositoy_ 创建仓库。
#### 2.启用Pages
在仓库顶部菜单中点击 _Settings_ ，进入仓库的设置界面，在左侧找到 _Pages_ 并点击进入Pages设置界面，点击 _Deploy from a branch_ 并选中Github Actions。
#### 3.开始写作
在仓库的顶部菜单栏找到 _Issues_ ，点击右边绿色按键 _New issue_ ，在 _Add a title_ 输入栏中，输入你的文章的标题，在 _Add a description_ 输入你的文章内容，在编辑完成后，在右边 _Label_ 标签类型选择栏中，选择 _documentation_ ，然后点击右下角 _create_ 绿色按钮，自动创建博客内容，你可以在仓库顶部菜单找到 _Actions_ 查看博客内容的构建进度，若报错，可以点击左侧_build Gmeek_ 选项，在右边出现的蓝色框中，找到Run workflow下拉菜单再点击Run workflow绿色按钮进行手动全局生成。
#### 4.访问博客界面
仓库顶部菜单中点击 _Code_ ，回到源码界面，向下翻找到 _README_板块，出现了蓝色的链接 `xxx.github.io` 点击，即可访问博客界面。
#### 5.修改配置文件
回到仓库源码界面，找到 _config.json_ 文件，其中必填参数有`title`（博客标题），`subTitle`（博客描述&自述），`avatarUrl`（博客头像），`GMEEK_VERSION`（Gmeek版本，一般写last也可以用具体tag版本）；其他选填参数可以在作者编写的 https://blog.meekdai.com/post/Gmeek-kuai-su-shang-shou.html 中自行查询

---

ending~
