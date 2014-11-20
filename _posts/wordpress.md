title: WordPress固定链接设置的几种方法
categories: 网络工具
tags:
  - 学习
  - 安装
  - 网络工具
  - 资讯
id: 227
date: 2014-09-02 16:19:37
---

传说中，固定链接有SEO功能，今天试了试，现在给大家分享一下：
wordpress固定链接设置技巧：
1、不要让日期出现在固定链接里面
　　这基于两个方面的考虑。一是如果数字出现在固定链接里面，等于提醒搜索引擎，这是很旧的内容了，没必要再爬一遍了。另外一个原因是，假如你要修改文章的日期重新发布的话，链接地址就变了，也就是意味着你的反向链接，PR 等等都没有了。
2、不要让分类的链接出现在固定链接里面
　　这一点是很多人都会忽略的地方。让分类出现在固定链接里面有两个缺陷：一是一篇文章如果选择了多个分类的话，则会出现多个链接地址，这很容易造成因为重复内容而被搜索引擎惩罚；二是有可能会造成关键词堆砌而被搜索引擎惩罚。
3、链接不要过深
　　这一点经常看到。很多wordpress 用户的固定链接是年/月/日/分类名/文章名。这种过于深的固定链接对搜索引擎是非常不友好的。
4、不要让中文字符出现在固定链接里面
　　虽然现在的搜索引擎已经能识别URL地址里面的中文字符，但无论是从美观上，还是从wordpress 优化的角度来看，都是非常差的。
wordpress固定链接设置的一些参数：
%year%：基于文章发布的年份，比如2010；
%monthnum%：基于文章发布的月份，比如01；
%day%：基于文章发布当日，比如06；
%hour%：基于文章发布小时数，比如23；
%minute%：基于文章发布分钟数，比如43；
%second%：基于文章发布秒数，比如33；
%postname%：基于文章的postname，其值为撰写时指定的缩略名，不指定缩略名时是文章标题；
%post_id%：基于文章post_id，比如48；
%category%：基于文章分类，子分类会处理成“分类/子分类”这种形式；
%author%：基于文章作者名。
　　将上述参数进行组合，即可得到wordpress的固定链接形式。
网上常见的几种设置方法：
•/%year%/%monthnum%/%day%/%postname%/

•/%year%/%monthnum%/%postname%/

•/%year%/%monthnum%/%day%/%postname%.html

•/%year%/%monthnum%/%postname%.html

•/%category%/%postname%.html

•/%post_id%.html
总结：最好的 wordpress固定链接形式是：域名/文章 名（参数为/%postname%.html）。
PS：原文作者已经说明最好参数，可本人觉得用/%post_id%.html 最简洁了。
注：本站采用/%post_id%.html