---
title:  "个人信息&affiliation"
modified: 2018-07-04 T16:03:49-04:00
categories: 
  - 界面设计
tags:
  - 笔记
---

{% include base_path %}

{% include toc title="目录" %}


## 界面设计的第一篇笔记

### 个人信息编辑
1.打开config.yml

2.在下面图片中修改个人信息

![修改个人信息](https://gitee.com/NFUNM030/minimal-mistakes/raw/master/images/%E4%BF%AE%E6%94%B9%E4%B8%AA%E4%BA%BA%E4%BF%A1%E6%81%AF.png)

*注意url和头像地址都要写正确，不然会出现404*


### 增加affiliation

1.打开config.yml，找到第25行

![在config里增加affiliation](https://gitee.com/NFUNM030/minimal-mistakes/raw/master/images/%E5%9C%A8config%E9%87%8C%E5%A2%9E%E5%8A%A0affiliation.png)

2.在repository和teaser之间，增加一行affiliation【可复制老师格式，注意修改】

3.修改成自己的内容，文本直接在引号内增加，不用写<p>标签

4.打开includes里面的footer.html，在最下面增加一行代码来声明版权：来自jekyll&minimal-mistakes

<div class="page__footer-copyright">{{ site.affiliation }}  <br/> &copy; {{ site.time | date: '%Y' }} {{ site.name | default: site.title }}. {{ site.data.ui-text[site.locale].powered_by | default: "Powered by" }} <a href="https://jekyllrb.com" rel="nofollow">Jekyll</a> &amp; <a href="https://mademistakes.com/work/minimal-mistakes-jekyll-theme/" rel="nofollow">Minimal Mistakes</a>.</div>

5.完成，网站显示如下

![网站中的affiliation](https://gitee.com/NFUNM030/minimal-mistakes/raw/master/images/%E7%BD%91%E7%AB%99%E4%B8%AD%E7%9A%84affiliation.png)
