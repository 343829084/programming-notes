# 编程开发

## 编程工具链

工欲善其事，必先利其器。以下就编程工具链推荐一些效率型工具。

### 文本编辑器

在节[不会Coding如何破？](../chapter3-advanced-programming-part1/README.html#sec-coding)中提到：「一旦算法（伪代码）描述齐备，程序编写不过是打字校对的工作。」咱们平时学习工作都非常讲究效率，那么「打字校对」的工作是不是也可以也有一些比较好的办法来提高效率呢？答案是肯定的！一些聪明的程序员早已想好了各种办法来提高Coding的效率，其中之一便是选择一款适合自己的高效Text Editor（用来输入程序代码的玩意儿，称为文本编辑器）。

Windows下大家最常见的恐怕就是记事本程序咯，够小巧，但我想应该没几个人愿意一直用这玩意儿吧？输几行代码进去它似乎什么反应也没有，代码高亮也没有。Linux 下最普通的便是 nano 了。不过比起下面即将出场的两位大神恐怕他们都得往一边站，OK,该轮到Vim和Emacs出场了。

* Vim-the god of editors
* Emacs-the god’s editor

#### Vim-Vi IMproved

Vim是从vi发展出来的一个文本编辑器。代码补全、编译及错误跳转等方便编程的功能特别丰富，在程序员中被广泛使用。开始学习的时候可能会进展缓慢，但是一旦掌握一些基本操作之后，能大幅度提高编辑效率。左耳朵耗子写的[Vim系列教程](http://coolshell.cn/tag/vim)十分不错。其中最适合入门的非[简明 Vim 练级攻略](http://coolshell.cn/articles/5426.html)莫属。下面放一张[给程序员的VIM速查卡](http://coolshell.cn/articles/5479.html#more-5479).

![Vim-cheat-sheet](../images/vim_cheat_sheet_for_programmers_print.png)

最后再力荐下BeiYuu的[Git时代的VIM不完全使用教程](http://beiyuu.com/git-vim-tutorial/)，使用Vundle管理Vim插件太惬意了。

#### Emacs-Editor MACroS

Emacs即Editor MACroS（宏编辑器），是一种文本编辑器，在程序员和其他以技术工作为主的计算机用户中广受欢迎。由于我不是Emacs用户，相关入门教程啥的还请Emacs党补充...

#### Sublime Text

除了以上两款神器，最近几年还冒出了个新一代神器——[Sublime Text: The text editor you'll fall in love with](http://www.sublimetext.com/)。简洁美观，上手特别容易，第三方插件也是异常丰富！觉得 Vim 和 Emacs 学习曲线太抖的可以尝试下这款性感的编辑器，不过得小声地说一句这款编辑器是商业软件，虽然可以免费使用。

### 版本控制

文本编辑器很好地解决了码字的问题，于是另一个问题来了——在一个项目的开发过程中需要和很多人一起合作，而且随着时间的推进代码会产生多个不同的版本。比较直观的想法是用文件名重命名的方式管理，如`file0.c, file1.c...`, 稍微好点的会用`file-2014-10-05.c...` 这种版本管理方式对于稍微有点规模的项目来说就显得有点太naive了，再说自己改着也蛋疼乳酸是不是？聪明的程序员早已为你想好了解决办法——Version Control(版本控制)! 专业的事情就应该交给专业的工具去解决。于是另一个问题又来了——**版本控制工具那么多，到底哪家强？蓝翔貌似没有版本控制工具啊...** 随便一搜就能发现以下几种：

1. [Git](http://zh.wikipedia.org/wiki/Git)
2. [Subversion](http://zh.wikipedia.org/wiki/Subversion)
3. [Mercurial](http://zh.wikipedia.org/wiki/Mercurial)

整体来讲，版本控制可以分为两种，分布式的和非分布式的 ←\_← 非分布式的可以理解为集中式的，也就是说在使用时必须有一个集中式的服务器。就像军训训练时出队必须向排长报告，这个排长就相当于集中式版本控制工具中的服务器啦。你想啊，你做什么都需要向排长报告，自然是相当不爽对不对π\_π 其中的代表就是Subversion啦。

如果这个版本控制的服务器离你十万八千里，而这时恰好某位熊孩纸有事没事拔掉你的网线，摁下路由器的开关——总之就是不能让你不能愉快的连接国外的服务器就是了，那么这个时候团队合作自然是无法愉快地进行下去了。既然和集中式版本控制做不成朋友，那就让我们和土豪分布式版本控制工具做朋友吧！弃Subversion，保平安～ 就连Subversion本身的开发也已于2014年愚人节转向使用git，噗哈哈哈，投票最后竟然通过了... [[svn1]](#ref-quit-sub) [[svn2]](#git-svn-diff) [[svn3]](#svn-april-fool)

#### 分布式版本控制工具 - git

分布式的好处在于，它可以不像集中式版本控制工具那样依赖中心服务器，开发完全可以在本地进行，不依赖网络。其中的代表就是[Git](http://zh.wikipedia.org/wiki/Git)啦。Git是 Linus Torvalds 继 Linux 之后给全人类带来的另一大神器，骚年颤抖吧！先放一张git在分支和合并方面的大杀器特性给大家醒醒脑，强大伐？

![Git-branch](../images/git-branch-1.png)

下面介绍一些Git方面的入门资料。

1. [git - 简明指南](http://rogerdudler.github.io/git-guide/index.zh.html)，目前见过的最简git指南，原来的英文版被翻译成了各种其他语言，漫画超友爱 ≖‿≖✧
2. [Git 简要教程](https://gist.github.com/bigeagle/3953973)，b哥整理的教程，简洁实用。
3. [Git分支管理策略](http://www.ruanyifeng.com/blog/2012/07/git.html)，阮一峰提供的针对Git分支管理策略。
4. [Git Magic](http://www-cs-students.stanford.edu/~blynn/gitmagic/intl/zh_cn/)，挺适合入门的教程，文字超友爱 ≖‿≖✧
5. [Pro Git](http://git-scm.com/book)，官方教程，非常全面，简单入门的话先看前几章就够用了。


## Notes

1. <a name="ref-quit-sub">[svn1]</a> [为什么我们要放弃Subversion](http://www.infoq.com/cn/articles/thoughtworks-practice-partiv)
2. <a name="git-svn-diff">[svn2]</a> [GIT和SVN之间的五个基本区别 | 外刊IT评论](http://www.vaikan.com/5-fundamental-differences-between-git-svn/)
3. <a name="svn-april-fool">[svn3]</a> [[INFRA-7524] April Fools: migrate Apache Subversion project over to the git repo - ASF JIRA](https://issues.apache.org/jira/browse/INFRA-7524)


### IDE vs Terminal

* * * * *

待整合完善

前边说了那么多编程的东西，那么怎么把自己的想法变为最终的结果呢？——当然是选择合适的编译器（或者类似的东西）啦，首推GCC\#，关于编译器在这就不多介绍了，前边已经做过初步解释，初学者无需在此浪费过多时间，知道它能把你的代码翻译为计算机可执行的文件就OK了。下边针对C/C++做些介绍，其它语言类似。

就国内的高校C语言教学来说，Windows下的VC6.0使用率还是比较广的，估计大部分都是用的盗版汉化软件，我大一一开始学的时候老师上课演示也是用VC6.0示范的，不得不在这里小小的抗议一下，初学编程完全无需VC6.0(在Win7下兼容性很成问题)甚至Visual Studio这样的庞然大物，光建工程配置文件就能打击一大批新手的自信心，而且莫名其妙的错误是经常会有的！对于初学者，个人觉得Linux + Terminal就非常不错，能配合《Linux C一站式编程》就更完美了。

如果你喜欢IDE，那也没关系，免费开源的[<http://zh.wikipedia.org/wiki/Code>::Blocks Code::Blocks]，自由小巧的[Dev-C++](http://zh.wikipedia.org/wiki/Dev-C%2B%2B)也不错，如果你平时使用多种语言开发，开源的Eclipse当仁不让。当然咯，如果你钟情于Windows，Visual Studio则比较适合你，初学时可以用免费的Express版，也可以使用微软授权给高校学生授权的Professional版本。

另外值得一提的就是软件调试，这本是一块很大的话题，《Linux C一站式编程》中有关gdb的使用已经很详细了，有兴趣的去看看，其它IDE或多或少也有类似的排错功能，使用方法见各软件帮助文档或网络上的教程。

除了IDE这种开发方式，你也可以使用前边提到过的Text Editor配合编译器使用，配置好的话熟练后非常方便，效率也较高。更多的介绍请参考Wikipedia或者社区wiki之[工具篇](如何用C/C++做工程 "wikilink")。
