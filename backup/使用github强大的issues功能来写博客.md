原文：https://github.com/zp1112/blog/issues/3

目前写博客是使用hexo部署，好处在于可以定制博客风格，没有设计感的人就别说定制了，定制了也很丑，只好用模板。要使用图片什么的还得上传到图床然后粘贴，写好了还得部署。还是挺麻烦的，比较适合写那种深入理解的文章。自从多说那个很丑的评论系统关闭了以后，大家纷纷替换了disqus评论系统，好像要翻墙？还得，注册才能评论？总之各种不方便。

另外一个记笔记的是印象笔记，他的优点先不说了，最大的缺点是，笔记太零散，回头找的时候已经找不到当初的那个知识点了。

还尝试了一个在线文档编辑，[石墨文档](https://shimo.im/)，讲真这玩意还不错，但是也存在一个毛病，就是知识多了，文件创建多了，就找不到知识点了、、、

作为程序员，大多数人写博客，一方面想要让自己的博客精美，一方面又想让自己的博客得到传播，好成为大佬一样的网红前端，噗。。。

但是我们在平时工作或者阅读的时候，经常会遇到一些有意思的问题，和有意思的知识点，这时候想要即兴写一篇总结和笔记，又不想过段时间找不到。那么github的issues可以派上用场了，

优点：
图片直接上传，使用github的静态服务
支持markdown
github自带issues评论系统，还都是gay界各路大佬，可以共同审查博客中暴露的问题，帮助进步。
labels等同于是博客的tag标签，明显
projects等同于是博客的分类，整洁
issues列表就是博客归档，一目了然

那么我就从零开始使用github issues搭建属于自己的博客吧。

第一步，新建一个仓库

可以命名为blog或者自己喜欢的名字。

image

第二步，新建project
这里的project可以类比分类，将来你写好的issue可以拖到某个你已经创建的分类下面。比如新建了github专题的，以后有关github的文章都可以拖到这里。

image

第三步，新建issue
在右侧点击label的标志，可以选择已创建的一些label，或者当场创建label，需要注意label太散也不好，久了也会造成知识太零碎的情况。

image

选择一个project，提交后这个issue就会分类到这个project下面

image

然后点击提交issue试试

结果

最后你会在issues列表里面看到很舒服的一条issue
image

进入projects的github专题，你会看到你还没创建子类，任务卡，相当于大专题里的小专题吧。

image

那么我们就新建一个，命名为_github博客搭建_
然后点击右上角的add cards,将新创建的一个issue拖到新建的github博客搭建这个类目下面

image

这个以后找文章就方便多了。其实各种各样的工具都是为了我们能够更好地做到碎片知识积累和查找。其实也避免不了知识多了分类零散的问题，最本质的还是要自己自觉地维护好知识点的分类。

最后一步，创建主页

首先在项目的根目录下新建两个文件
CNAME 该文件写上你要使用的域名
README.md 该文件使用markdown语法写上你的博客的简介，链接等。
然后打开settings->github pages选择分支
image
选择主题
image
image
选好后你的readme就会被渲染成这种风格的html主页。成功后会显示绿色的已成功并且可以勾上https。
然后访问你的域名，就可以看到你的readme啦。