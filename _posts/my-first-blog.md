title: 你好，独立博客
date: 2015-09-20 01:15:06
categories: diary
tags: blog
---

**如果能看到这里，说明你是一个帅哥或者美女。**

----------



# 我为什么要弄独立博客



其实我在CSDN上面有个博客，经常会转载一下有用的资料或者笔记什么的，但是总感觉那是别人的地盘，没有什么归属感。  
而最近查一些资料，经常能逛到别人的独立博客上面，所以我就想：为什么我不弄一个独立博客，如果我有了个人博客，哦呵呵，那么我不仅可以装逼，还可以装逼，甚至还可以装逼了呢，想想还有点小激动噶~  
**装逼是其次，主要还是想提升一下自己的技术啦（认真脸）**


----------

# 博客怎么搭建的


网上有很多相关的教程，我就不班门弄斧说具体步骤了。捣鼓了两个晚上，终于能在实验室和寝室不同的机器上更新博客了。



- 建站工具，选择了Hexo，我主要是参考了[Hexo系列教程][1]和[Hexo你的博客][2]，
为什么用Hexo？看看作者的介绍你就知道了：	
	> 不可思议的快速 ─ 只要一眨眼静态文件即生成完成
	支持 Markdown
	仅需一道指令即可部署到 GitHub Pages 和 Heroku
	已移植 Octopress 插件
	高扩展性、自订性
	兼容于 Windows, Mac & Linux`

- 域名购买，没有悬念选择狗爹。花了不到10刀，买到[feipeng.info][3]这个域名，没拿到.cn和.me还是有点遗憾。

- 托管，github和gitcafe都可以，但我没用过gitcafe。

- Markdown，我也刚学这个玩意儿，写博客必备，用的是[cmd在线编辑器][4]。


----------

# 遇到的问题

为了在寝室也能更新博客，于是在笔记本上也安装了Hexo环境，一切准备就绪，SSH各种连接无误，无奈每次部署都显示
`Error:Permission denied (publickey).`
`fatal:Could not read from remote repository.`

好吧，我重新添加了一万次SSH key，依然无果，哔了动物园了。
灵机一动，想到一法，每次部署前手动打开一次SSH客户端：

   `$ eval $(ssh-agent -s)`  
   `$ ssh-add ~/.ssh/id_rsa`  

至此解决困扰一天的问题。

----------

# 我会怎么用博客

花了钱和精力，当然得用下去，我会分享一下有价值的资料，同时自己也会总结一些技术性的文章，写写随笔什么的~





  [1]: http://zipperary.com/categories/hexo/
  [2]: http://ibruce.info/2013/11/22/hexo-your-blog/
  [3]: http://feipeng.info
  [4]: https://www.zybuluo.com/mdeditor