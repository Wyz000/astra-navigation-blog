Differential Robotics Team — bilingual technical blog

Published page / 在线博客
https://wyz000.github.io/astra-navigation-blog/

HOW TO EDIT TEXT / 如何自己修改文字

1. 登录 GitHub，打开下面的文件，点击铅笔 Edit：
   https://github.com/Wyz000/astra-navigation-blog/blob/main/index.html
   此独立仓库的根目录 index.html 就是博客页面。

2. 在编辑器中搜索需要修改的原句，只修改文字，保留 HTML 标签、
   id、链接及引号、反斜杠等代码结构。
   当前正文有三份：
   - <article id="article"> 内是默认英文 HTML；
   - const ARTICLES 的 en 是切换到英文时使用的内容；
   - const ARTICLES 的 zh 是切换到中文时使用的内容。
   因此修改英文正文一般需要同步改两处；中文正文改 zh 中的一处。
   中英文不会自动互译，需要分别修改。
   ARTICLES 内是 JavaScript 字符串，保留现有的转义引号。新增英文
   双引号时要写成反斜杠加双引号，或使用弯引号 “ ”。

3. 点击 Commit changes，写简短说明，例如 Update navigation text，
   选择 Commit directly to the main branch，再确认提交。

4. 打开 Actions，等待 pages build and deployment 显示绿色成功：
   https://github.com/Wyz000/astra-navigation-blog/actions
   再刷新博客检查中英文。若浏览器仍显示旧内容，可强制刷新。

IMAGES / 图片

当前第一张地图：assets/figure-01.jpg。
其他研究图片和视频位于 assets/ 文件夹。
替换图片时可以上传同名同格式文件覆盖；改文件名时要同步修改
默认英文 HTML、ARTICLES.en 和 ARTICLES.zh 的对应路径。

LAYOUT / 布局

桌面端目录在左侧固定显示；窄屏目录移到文章顶部。
英文默认显示，EN / 中文切换会记住语言选择。
分享链接可使用 ?lang=en 或 ?lang=zh。
全文包含三个研究章节、结语、8张配图、15段录像和10条参考文献。
