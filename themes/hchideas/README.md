[![Build Status](https://travis-ci.org/hexojs/hexo.svg?branch=master)](https://travis-ci.org/hexojs/hexo)  [![NPM version](https://badge.fury.io/js/hexo.svg)](http://badge.fury.io/js/hexo) [![Coverage Status](https://coveralls.io/repos/hexojs/hexo/badge.svg?branch=master)](https://coveralls.io/r/hexojs/hexo?branch=master) [![Build status](https://ci.appveyor.com/api/projects/status/hpx3lduqjj2t6uqq/branch/master?svg=true)](https://ci.appveyor.com/project/tommy351/hexo/branch/master) [![Gitter](https://badges.gitter.im/hexojs/hexo.svg)](https://gitter.im/hexojs/hexo?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

# 关于这个博客主题 Hexo-Theme 使用


随着hexo的版本升级，同时我也想重构我的旧版博客主题，因此在这个月对博客进行了重构加改版，这个仓库存放我的新博客，并且我也会一直使用这个主题。目前基本改版完成，后续可能还会有些细节上的修补。

**本博客访问地址：[小神童博客](http://btchandbook.com)**。

----------

# Hexo-Theme 使用


## 安装

	$ git clone https://git.coding.net/yeechong/Hexo-Theme-Buer.git

## 配置

修改hexo根目录下的 _config.yml ： theme: Hexo-Theme-Buer


## 更新

	cd themes/buer
	git pull


# 配置

关于配置文件，主题配置文件在主目录下的_config.yml：_config.yml

相关插件的安装：请参照[Hexo插件安装](http://11)

## 全部功能

```html
# >>> Basic Setup | 基础设置 <<<

# Header | 主菜单
## About Page: `hexo new page about`
## Tags Cloud Page: `hexo new page tags`
menu:
  #开始的地方: 
  # 博客主页: /
  博文目录: /archives
  拙作: /works
  留下点什么: /about
  #导航: 
  # 静心阅读: /tags
  # 光影之路: /instagram
  # 随笔: /tags/随笔

# Link to your avatar | 填写头像地址
avatar: img/head.jpg

# Small icon of Your site | 站点小图标地址
favicon: img/favicon.png

# Social info. Bar | 社交信息展示
## Keep "mailto:" in Email | 设置 Email 时保留 "mailto:"
## Encrypt email 加密邮件地址 http://ctrlq.org/encode/
## RSS requires a plugin to take effect | 使用 RSS 需先安装对应插件
## https://github.com/hexojs/hexo-generator-feed
subnav:
  mail: "mailto:xxx@gmail.com"
  github: "https://github.com/xxx"
  # zhihu: "#"
  #weibo: ""
  # google: "#"
  #twitter: "#"
  #linkedin: "#"
  # facebook: "#"
  rss: /atom.xml
  # pinterest: "#"
  # QQ: "#"
  # wechat: "#"
  # douban: "#"
  # pinboard: "#"
  # stackoverflow: "#"
  # Instagram: "#"
  # segmentfault: "#"

# >>> Conments 评论系统 <<<
# Chose ONE as your comment system and keep others disable.
# 选一个作为网站评论系统，其他保持禁用。

disqus: 
  #on: true
  shortname: 
  # https://help.disqus.com/customer/en/portal/articles/466208-what-s-a-shortname-
  # It is unnecessary to enable disqus here if 
  # you have set "disqus_shortname" in your site's "_config.yml" 

duoshuo: 
  on: true
  domain: yeechong
  # 是否开启多说评论，http://duoshuo.com/create-site/
  # 使用上面网址登陆你的多说，然后创建站点，在 domain 中填入你设定的域名前半部分
  # http://<要填的部分>.duoshuo.com (domain只填上<>里的内容，不要填整个网址)

youyan:
  #on: true
  id: 
  # 是否开启友言评论，http://www.uyan.cc/index.php
  # id 中填写你的友言用户数字ID，注册后进入后台管理即可查看
  # 友言服务在 Web 环境下运行，普通本地环境无法查看，请部署后在线上测试。


# >>> Style Customisation 样式自定义 <<<

# Background | 网页侧边栏背景
## "background_sum": show images form /source/background/的图片数目
## "on: true": 自动随机显示这5张图片
## "on: false": 自定义显示图片设置background_image: 5
background:
  on: true
  #on: false
  background_sum: 27
  background_image: 109

highlight_style:
  on: true
  inline_code: 5
  code_block: 5
  # Set inline_code to style highlight text
  # Chose a highlight theme for code block
  # 通过 inline_code 切换内置文本高亮样式 Value: 0 - 9 可选
  # 通过 code_block 切换内置代码高亮配色主题  Value: 0 - 4 

blockquote_style:
  #on: true
  blockquote: 1  
  # Value: 0 - 7 可选
  # 自定义文章「引用部分」的样式

# 左边栏宽度 px
left_col_width: 300

# 目录中标题不换行
# Keep TOC title on the same line | 
toc_nowrap: false

# 自定义"阅读全文"链接按钮的显示文字
# Customize the text on excerpt link
excerpt_link: Yeechong 
#修改more>>的文字

# 是否显示边栏中的搜索框（仅样式，未添加搜索功能）
# Search Box in left column
search_box: true

# 是否开启主页及加载头像时的动画效果
# Animation in Homepage and Loading avatar
animate: true


# >>> Small features | 小功能设置 <<<

# 是否开启边栏多标签切换
# Birdhouse button in left column
tagcloud: true

# Blogroll, Link exchange | 友情链接
# friends: false
friends:
  yeechong: http://buer.website/
  不二: http://buer.website/
  

#是否开启“关于我”。
aboutme: xxx。
#aboutme: false

# 是否在新窗口打开链接
# Open ALL link in a new tab
# open_in_new: false
open_in_new: true

# Customize feed link 自定义订阅地址
rss: /atom.xml


# >>> Vendors | 第三方工具 & 服务 <<<

# images viewer | 图片浏览器
## http://www.fancyapps.com/fancybox/
fancybox: true

# Display Math(LaTeX, MathML...) | 数学公式支持
## https://www.mathjax.org/
mathjax: false

# Socail Share | 是否开启分享
# share: true
baidushare: true

# 开启后页面变的模糊
# showshare: true

# 百度、谷歌站长验证。填写 HTML 标签 content
# Site Verification for Google and Baidu. HTML label content.
google_site: # pFW527fHrjfI0si2w4NQ0w3cTw12AvvuohAu1PUfqKA
baidu_site: #c167b9feb4f0b208b712c79629c188e4

# Fill in Google Analytics tracking ID, #e.g. UA-XXXXX-X, or Baidu Analytics hash key
google_analytics:
baidu_analytics:

# 不蒜子网站计数设置
# http://ibruce.info/2015/04/04/busuanzi/
visit_counter:
  on: true
  site_visit: XX到访数
  page_visit: 本页阅读量

# A标签提示
TipTitle: true

# Loading  
# why me?
Loading: true
```

## 文章markdown属性

```
title: 前端知识体系
date: 2016-01-16 13:58:41
description: #描述
categories: #分类
- HTML 书籍
- HTML 书籍
tags:
- HTML 标签 
- HTML 标签
toc: true 文章目录
author:
comments:
original:
permalink: 
---
　　** 知识体系：**<Excerpt in index | 首页摘要> 

+ <!-- more -->
<The rest of contents | 余下全文>

```

### 我使用的格式：

```
title: Markdown-文章格式
date: #默认系统时间
description: #描述
categories: #分类
- HTML 书籍
- HTML 书籍
tags:
- HTML 标签 
- HTML 标签
toc: true 文章目录
author: #
comments: true #是否开启评论true
original:
permalink: demo #url中的名字    文件名
---

　　** 知识体系：**<Excerpt in index | 一盏灯， 一片昏黄； 一简书， 一杯淡茶。 守着那一份淡定， 品读属于自己的寂寞。 保持淡定， 才能欣赏到最美丽的风景！ 保持淡定， 人生从此不再寂寞。> 

+ <!-- more -->  #同wordpress一样，<!--more-->之上的内容为摘要。
```
## 404 Page

```
hexo new page 404
And then set permalink: /404 in /source/404/index.md front matter.
在 Hexo 中创建匹配主题的404页面
```

# 主题结构

```
.
├── languages            #多语言
|   ├── default.yml      #默认语言
|   └── zh-CN.yml        #中文语言
├── layout               #布局，根目录下的*.ejs文件是对主页，分页，存档等的控制
|   ├── _partial         #局部的布局，此目录下的*.ejs是对头尾等局部的控制
|   └── _widget          #小挂件的布局，页面下方小挂件的控制
├── source               #源码
|   ├── css              #css源码 
|   |   ├── _base        #*.styl基础css
|   |   ├── _partial     #*.styl局部css
|   |   ├── fonts        #字体
|   |   ├── images       #图片
|   |   └── style.styl   #*.styl引入需要的css源码
|   ├── fancybox         #fancybox效果源码
|   └── js               #javascript源代码
├── _config.yml          #主题配置文件
└── README.md            #用GitHub的都知道
```
# 主题首页显示概要设置

在首页显示一篇文章的部分内容，并提供一个链接跳转到全文页面是一个常见的需求。 NexT 提供三种方式来控制文章在首页的显示方式。 也就是说，在首页显示文章的摘录并显示 阅读全文 按钮，可以通过以下方法：
1. 在文章中使用 <!-- more --> 手动进行截断，Hexo 提供的方式 推荐
2. 在文章的 front-matter 中添加 description，并提供文章摘录
3. 自动形成摘要，在 `主题配置文件` 中添加：

```cpp

```

# 博客名字欢迎语

位置： \layout\_partial\left-col.ejs(13):          

```
<h1 class="header-author"><a href="<%- config.root %>" title="Hi Mate"><%=theme.author%></a></h1>
```


# 底部导航修改页面 

文件位置：layout\_partial\footer.ejs

# 分享按钮

```
以下代码是百度分享的页面24页面分享的代码，可以自行选择以下标签。

配置

vim themes/light/layout/_partial/article.ejs
删除
<%-partial('post/share')%>
替换为刚刚获取的分享代码

<div class="bdsharebuttonbox">
    <a href="#" class="fx fa-weibo bds_tsina" data-cmd="tsina" title="分享到新浪微博"></a>
    <a href="#" class="fx fa-weixin bds_weixin" data-cmd="weixin" title="分享到微信"></a>
    <a href="#" class="fx fa-qq bds_sqq" data-cmd="sqq" title="分享到QQ好友"></a>
    <a href="#" class="fx fa-facebook-official bds_fbook" data-cmd="fbook" title="分享到Facebook"></a>
    <a href="#" class="fx fa-twitter bds_twi" data-cmd="twi" title="分享到Twitter"></a>
    <a href="#" class="fx fa-linkedin bds_linkedin" data-cmd="linkedin" title="分享到linkedin"></a>
    <a href="#" class="fx fa-files-o bds_copy" data-cmd="copy" title="分享到复制网址"></a>

    <a href="#" class="fx fa-plus-square bds_more" data-cmd="more"></a>
    <a href="#" class="fx fa-tencent-weibo bds_tqq" data-cmd="tqq" title="分享到腾讯微博"></a>
    <a href="#" class="fx fa-renren bds_renren" data-cmd="renren" title="分享到人人网"></a>
    <a href="#" class="fx fa-paw bds_tieba" data-cmd="tieba" title="分享到百度贴吧"></a>
    <a href="#" class="fx fa-envelope-o bds_mail" data-cmd="mail" title="分享到邮件分享"></a></div>
    <a href="#" class="fx fa-print bds_print" data-cmd="print" title="分享到打印"></a>
    <a href="#" class="fx fa-share-alt bds_mshare" data-cmd="mshare" title="分享到一键分享"></a>
    <a href="#" class="fx bds_douban" data-cmd="douban" title="分享到豆瓣网"></a>
    <a href="#" class="fx fa- bds_qzone" data-cmd="qzone" title="分享到QQ空间"></a>
    <a href="#" class="fx fa- bds_evernotecn" data-cmd="evernotecn" title="分享到印象笔记"></a>
</div>
<script>window._bd_share_config={"common":{"bdSnsKey":{},"bdText":"","bdMini":"1","bdMiniList":false,"bdPic":"","bdStyle":"2","bdSize":"24"},"share":{}};with(document)0[(getElementsByTagName('head')[0]||body).appendChild(createElement('script')).src='http://bdimg.share.baidu.com/static/api/js/share.js?v=89860593.js?cdnversion='+~(-new Date()/36e5)];</script>

```
# 修改样式

```
source\css\_partial\article.styl

/* bd share button box */
.bdshare-button-style2-24{
  width: 330px;
  margin: auto;
  .fx {
      color: #999;
      padding: 0;
      margin: 6px;
      height: 54px;
      display: inline-block;
      font: normal normal normal 36px/1 FontAwesome;
      background: none;
      text-rendering: auto;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
  }
  .fx:hover{
    color: #FFF;
    opacity: 1;
  }
}

themes\spfk\source\css\_partial\mobile.styl
/* bd share button box */
.bdshare-button-style2-24{
  width: 289px;
  .fx {
      font: normal normal normal 30px/1 FontAwesome;
  }
}

```
# 百度统计

```
去百度统计获取统计代码

vim layout/_partial/baidu_analytics.ejs

<% if (theme.baidu_analytics){ %>

<script>
var _hmt = _hmt || [];
(function() {
  var hm = document.createElement("script");
  hm.src = "https://hm.baidu.com/hm.js?746094ae9897b0b9190120d1aae8747e";
  var s = document.getElementsByTagName("script")[0]; 
  s.parentNode.insertBefore(hm, s);
})();
</script>


<% } %>



vim Hexo_Theme_Buer/_config.yml

baidu_analytics: true
# hm.src = "https://hm.baidu.com/hm.js?746094ae9897b0b9190120d1aae8747e";
baidu_analytics_id: 746094ae9897b0b9190120d1aae8747e


vim Hexo_Theme_Buer/layout/_partial/head.ejs
在/head前添加

<%- partial('baidu_analytics') %>
</head>

```

# 不蒜子

```
/layout/_partial/footer.ejs

<footer id="footer">
    <div class="outer">
        <div id="footer-info">
            <div class="footer-left">
                &copy; <%= date(new Date(), 'YYYY') %> <%= config.author || config.title %>
            </div>
            <div class="footer-right">
                <a href="http://hexo.io/" target="_blank">Hexo</a>  Theme <a href="https://github.com/luuman/hexo-theme-spfk" target="_blank">spfk</a> by luuman
            </div>
        </div>
        <div class="visit">
            <span id="busuanzi_container_site_pv" style='display:none'>
                <span id="site-visit" >本站到访数: 
                    <span id="busuanzi_value_site_uv"></span>
                </span>
            </span>
            <span id="busuanzi_container_page_pv" style='display:none'>
                <span id="page-visit">, 本页阅读量: 
                    <span id="busuanzi_value_page_pv"></span>
                </span>
            </span>
        </div>
    </div><script async src="https://dn-lbstatics.qbox.me/busuanzi/2.3/busuanzi.pure.mini.js">
</script>
</footer>
```
# 页面上下导航

```
 scrolling-button.ejs

<div class="scroll" id="scroll">
    <a href="#"><i class="fa fa-arrow-up"></i></a>
    <a href="#comments"><i class="fa fa-comments-o"></i></a>
    <a href="#footer"><i class="fa fa-arrow-down"></i></a>
</div>
<script>
    $(document).ready(function() {
        if ($("#comments").length < 1) {
            $("#scroll > a:nth-child(2)").hide();
        };
    })
</script>

```
## 修改样式

```
Hexo-Theme-Buer\source\css\_partial\main.styl
#scroll{
    right: 0;
}

.scroll {
    z-index: 999;
    position: fixed;
    bottom: 40px;   //修改离底部的距离，可以在角落添加建议等底盘图标。
    text-align: center;
    line-height: 42px;
    a {
        display: block;
        width: 29px;
        height: 42px;
        font-size: 28px;
        &:last-child {
            border-bottom: none;
        };
        .fa {
            color: rgba(255, 255, 255, .8);
        }
        &:hover {
            background: rgba(147, 181, 224, .3) !important; 
            .fa {
                color: white;
            }
        }
    }
}
```

# 版权声明

```
\layout\_partial\post\nav.ejs

<% if (post.original != false && !is_page()){ %>
    <div class="copyright">
        <p><span>本文标题:</span><a href="<%- url_for(post.path) %>"><%= post.title %></a></p>
        <p><span>文章作者:</span><a href="/" title="请访问 <%=theme.author%> 博客"><%=theme.author%></a></p>
        <!-- <p><span>发布时间:</span><%= post.date.format("YYYY年MM月DD日 - HH时mm分") %></p> -->
        <!-- <p><span>最后更新:</span><%= post.updated.format("YYYY年MM月DD日 - HH时mm分") %></p> -->
        <p>
            <span>原始链接:</span><a class="post-url" href="<%- url_for(post.path) %>" title="<%= post.title %>"><%= post.permalink %></a>
            <span class="copy-path" data-clipboard-text="原文: <%= post.permalink %>　　作者: <%=theme.author%>" title="点击复制文章链接"><i class="fa fa-clipboard"></i></span>
            <script src="/js/clipboard.min.js"></script>
            <script> var clipboard = new Clipboard('.copy-path'); </script>
        </p>
        <p>
            <span>许可协议:</span><i class="fa fa-creative-commons"></i> <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/cn/" title="中国大陆 (CC BY-NC-SA 3.0 CN)">"署名-非商用-相同方式共享 3.0"</a> 转载请保留原文链接及作者。
        </p>
    </div>
<% } %>

<% if (post.prev || post.next){ %>
<nav id="article-nav">
  <% if (post.prev){ %>
    <a href="<%- url_for(post.prev.path) %>" id="article-nav-newer" class="article-nav-link-wrap">
      <strong class="article-nav-caption"><</strong>
      <div class="article-nav-title">
        <% if (post.prev.title){ %>
          <%= post.prev.title %>
        <% } else { %>
          (no title)
        <% } %>
      </div>
    </a>
  <% } %>
  <% if (post.next){ %>
    <a href="<%- url_for(post.next.path) %>" id="article-nav-older" class="article-nav-link-wrap">
      <div class="article-nav-title"><%= post.next.title %></div>
      <strong class="article-nav-caption">></strong>
    </a>
  <% } %>
</nav>
<% } %>
```
## 修改版权框样式

```
Hexo-Theme-Buer\source\css\_partial\article.styl

/* copyright */
.copyright {
    width: 85%;
    max-width: 45em;
    margin: 0 auto;
    padding: .5em 1.8em;
    border: 1px solid lightgray;
    font-size: .93em;
    line-height: 1.6em;
    word-break: break-word;
    background: rgba(255, 255, 255, .4);
    span {
        margin-right: 1em;
        color: #B5B5B5;
        font-weight: bold;
    }
    a {
        color: gray;
        &:hover {
            font-weight: bold;
            color: #a3d2a3;
            text-decoration: underline;
        }
    }
    &:hover p .copy-path::after {
        content: "复制";
    }
    .post-url:hover {
        font-weight: normal;
    }
    .copy-path {
        margin-left: 1em;
        &:hover {
            color: gray;
            cursor: pointer;
        }
    }
}
```
# 社交账号图标修改

```
\layout\_partial\left-col.ejs

<nav class="header-nav">
    <div class="social">
        <% for (var i in theme.subnav){ %>
            <a class="fl <%= i %>" target="_blank" href="<%- url_for(theme.subnav[i]) %>" title="<%= i %>"><%= i %></a>
        <%}%>
    </div>
</nav>

```
# 站点Swiftype搜索框

```
layout\_partial\left-col.ejs

<form>                
    <input type="text" class="st-default-search-input search" id="search" placeholder=" Search..." autocomplete="off" autocorrect="off" autocapitalize="off">
</form>


D:\Hexo\Hexo\themes\spfk\layout\_partial\after-footer.ejs

<script type="text/javascript">
  window.onload = function(){
    document.getElementById("search").onclick = function(){
        console.log("search")
        search();
    }
  }
  function search(){
    (function(w,d,t,u,n,s,e){w['SwiftypeObject']=n;w[n]=w[n]||function(){
    (w[n].q=w[n].q||[]).push(arguments);};s=d.createElement(t);
    e=d.getElementsByTagName(t)[0];s.async=1;s.src=u;e.parentNode.insertBefore(s,e);
    })(window,document,'script','//s.swiftypecdn.com/install/v2/st.js','_st');

    _st('install','A1Pz-LKMXbrzcFg2FWi6','2.0.0');
  }
</script>
```
## 修改样式

```
.search {
    width: 68%;
    height: 18px;
    margin-top: 1px;
    padding: 0;
    font-family: inherit;
    border: 2px solid transparent;
    border-bottom: 2px solid lightgray;
    border-radius: 2px;
    opacity: .7;
    background: none;
    &:hover {
        border: 0px solid lightgray;
        opacity: 1;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
    };
}


display: inline-block;
    width: 190px;
    height: 16px;
    padding: 7px 11px 7px 28px;
    border: 1px solid #bbb;
    border: 1px solid rgba(0,0,0,0.25);
    font-weight: 400;
    color: #444;
    font-size: 14px;
    line-height: 16px;
    box-sizing: content-box;
    background: #fff 8px 8px no-repeat url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA0AAAANCAYAAABy6%2BR8AAAACXB…Hx4Taq1nrnKaW8K6XUUsrHWuvNevdRRLzFGwzvDbXAB9cDAHvhedDruuxSAAAAAElFTkSuQmCC);
    background-clip: padding-box;
    -webkit-border-radius: 5px;
    -moz-border-radius: 5px;
    -ms-border-radius: 5px;
    -o-border-radius: 5px;
    border-radius: 5px;
    -webkit-box-shadow: none;
    -moz-box-shadow: none;
    box-shadow: none;
    font-family: "Helvetica Neue",Helvetica,Arial,"Lucida Grande",sans-serif;
```
# RSS插件

```
安装RSS插件

$ npm install hexo-generator-feed --save

    开启RSS功能

    编辑hexo/themes_config.yml，添加如下代码：

    rss: /atom.xml #rss地址  默认即可
```
# sitemap网站地图 插件

```
1、安装插件：

$ npm install hexo-generator-sitemap --save
$ npm install hexo-generator-baidu-sitemap --save

2、在博客目录的hexo/_config.yml中添加如下代码：

# 自动生成sitemap编辑

sitemap:
path: sitemap.xml
baidusitemap:
path: baidusitemap.xml

3、hexo编译的时候会自动在根目录生成站点地图

    UUhike@UUhike-pc MINGW64 /d/Hexo/Hexo (master)
    $ npm install hexo-generator-sitemap --save
    npm WARN install Couldn't install optional dependency: Unsupported
    npm WARN install Couldn't install optional dependency: Unsupported
    hexo-site@0.0.0 D:\Hexo\Hexo
    └── hexo-generator-sitemap@1.0.1


    UUhike@UUhike-pc MINGW64 /d/Hexo/Hexo (master)
    $ npm install hexo-generator-baidu-sitemap --save
    npm WARN install Couldn't install optional dependency: Unsupported
    npm WARN install Couldn't install optional dependency: Unsupported
    hexo-site@0.0.0 D:\Hexo\Hexo
    └── hexo-generator-baidu-sitemap@0.1.2


    UUhike@UUhike-pc MINGW64 /d/Hexo/Hexo (master)
    $ hexo g
    INFO  Files loaded in 2.42 s
    INFO  Generated: baidusitemap.xml
    INFO  Generated: sitemap.xml
    INFO  2 files generated in 477 ms
```

# 关于Hexo迁移

```
非常感谢Waterstrong


# URL #这项暂不配置，绑定域名后，欲创建sitemap.xml需要配置该项
## If your site is put in a subdirectory, set url as 'http://yoursite.com/child' and root as '/child/'
url: http://luuman.github.io/Blog/
root: /Blog/
permalink: :year/:month/:day/:title/
permalink_defaults:

上传是需要出入密码

# Deployment 站点部署到github要配置，上一节中已经讲过
## Docs: http://zespia.tw/hexo/docs/deploy.html
deploy:
  type: git
  #repository: git@github.com:luuman/Blog.git
  repository: https://github.com/luuman/Blog.git
  branch: gh-pages
```
# 多说插件

```
├── spfk
        ├── _config.yml #主题配置文件
    #是否开启多说评论，填写你在多说申请的项目名称 duoshuo: duoshuo-key（http://duoshuo-key.duoshuo.com/）
    #若使用disqus，请在博客config文件中填写disqus_shortname，并关闭多说评论
    duoshuo: true


复制到 themes\landscape\layout\_partial\article.ejs把

<% if (!index && post.comments && config.disqus_shortname){ %>
<section id="comments">
<div id="disqus_thread">
<noscript>Please enable JavaScript to view the <a href="//disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
</div>
</section>
<% } %>

改为

<% if (!index && post.comments && config.disqus_shortname){ %>
<section id="comments">
<!-- 多说评论框 start -->
<div class="ds-thread" data-thread-key="<%= post.layout %>-<%= post.slug %>" data-title="<%= post.title %>" data-url="<%= page.permalink %>"></div>
<!-- 多说评论框 end -->
<!-- 多说公共JS代码 start (一个网页只需插入一次) -->
<script type="text/javascript">
var duoshuoQuery = {short_name:'<%= config.disqus_shortname %>'};
  (function() {
    var ds = document.createElement('script');
    ds.type = 'text/javascript';ds.async = true;
    ds.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') + '//static.duoshuo.com/embed.js';
    ds.charset = 'UTF-8';
    (document.getElementsByTagName('head')[0] 
     || document.getElementsByTagName('body')[0]).appendChild(ds);
  })();
  </script>
<!-- 多说公共JS代码 end -->
</section>
<% } %>


```
修改样式：

[设计达人](http://www.shejidaren.com/use-css3-to-create-a-beautiful-comment-ui.html)

添加方法：
添加方法：打开「后台」 > 「多说评论」 > 「设置」 > 「基本设置」 > 然后把样式粘贴到「自定义CSS」文本框 > 「保存」

# 为Hexo博客添加目录

Hexo博客系统的核心支持生成目录（Table of Contents），但其默认的主题Landscape并不支持目录的显示。我们只需对Landscape的主题文件稍作修改并添加一点目录的CSS就可以在文章前面显示友好的目录了。
修改Landscape主题的ejs文件
我们首先要编辑文章显示页面的模板，也就是themes/landscape/layout/_partial/article.ejs文件。为了将目录生成在正文之前，我们首先在这个文件中找到<%- post.content %>，并在这一行之前加入如下代码：

```
引入文件_partial\article.ejs
    <% if (!index && post.toc != false && !is_page()){ %>
        <%- partial('_partial/toc') %>
    <% } %>


    <% if (!index && post.toc){ %>
    <%- partial('post/toc') %>
    <% } %>

<div id="toc" class="toc-article">
    <strong class="toc-title">文章目录</strong>
    <%- toc(post.content) %>
</div>
<style>
    .left-col .switch-btn {
        display: none;
    }
    .left-col .switch-area {
        display: none;
    }
</style>

<input type="button" id="tocButton" value="隐藏目录"  title="点击按钮隐藏或者显示文章目录">

<%- js('http://7.url.cn/edu/jslib/comb/require-2.1.6,jquery-1.9.1.min') %>
<script>
    var toc_button = document.getElementById("tocButton");
    var toc_div = document.getElementById("toc");
    toc_button.onclick=function() {
        if (toc_div.style.display == "none") {
            toc_div.style.display = "block";
            toc_button.value = "隐藏目录";
            document.getElementById("switch-btn").style.display = "none";
            document.getElementById("switch-area").style.display = "none";
        }
        else {
            toc_div.style.display = "none";
            toc_button.value = "显示目录";
            document.getElementById("switch-btn").style.display = "block";
            document.getElementById("switch-area").style.display = "block";
        }
    }

    if ($(".toc").length < 1) {
        $("#toc").css("display","none");
        $("#tocButton").css("display","none");
        $(".switch-btn").css("display","block");
        $(".switch-area").css("display","block");
    }
</script>

<% if (theme.toc_nowrap) { %>
    <style>
        .toc {
            white-space: nowrap;
            overflow-x: hidden;
        }
    </style>

    <script>
        $(document).ready(function() {
            $(".toc li a").mouseover(function() {
                var title = $(this).attr('href');
                $(this).attr("title", title);
            });
        })
    </script>
<% } %>
```
if语句中有两个条件，!index是为了不在首页的文章摘要中生成目录，post.toc确保了只在显式地标记了toc: true的文章中生成目录。若这两个条件满足，则创建一个目录的。
修改完这个文件之后，找一篇包含了多个子标题的文章，并在文章开头的front-matter中添加一句toc: true，在浏览器中访问这篇文章，应该可以看到文章的开头处已经有了带链接的目录。但是这样的目录实在太难看，我们还需要添加相应的CSS来将其指定为我们想要的样式。

## 目录样式


```
/*toc*/
#tocButton {
    position: fixed;
    border: none;
    left: 220px;
    top: 382px;
    background: none;
    font-size: .9em;
    font-weight: bold;
    color: lightgray;
    cursor: pointer
    font-family: inherit;
    outline: none; /*Remove button border when clicked.*/
    -webkit-appearance: none; /*Remove iOS button style*/
    &:hover {
        color: #88acdb;
    }
}
.toc-article {
  position: fixed;
  width: 230px;
  top: 378px;
  bottom: 1em;
  left: 0;
  margin-left: 0em;
  padding: 6px 10px 10px 50px;
  border-radius: 2.8%;
  overflow: auto;
}
#toc {
    float: right;
    font-size: .9em;
    line-height: 1.65em;
    z-index: 12;
    a {
        color: gray;
        &:visited {
            color: rgba(244, 131, 133, 1);
        } 
        &:hover {
            color: #88acdb;
            text-decoration: none;
        }
    }
    li:hover {
        background: none;
        li:hover {
            background: rgba(158, 188, 226, .21);
        }
    }
    .toc-title {
        font-weight: bold;
        color: gray;
    }
    .toc {
        padding: .7em;
        padding-right: 0;
        li {
            list-style-type: none;
        }
    }
    ol {
        margin-left: 0;
    }
    .toc-child {
        padding-left: 1.25em;
        margin: 4px 0; 
    }
    .toc-link:hover {
        background: rgba(158, 188, 226, .21);
    }
}

.copyright {
    width: 85%;
    max-width: 45em;
    margin: 0 auto;
    padding: .5em 1.8em;
    border: 1px solid lightgray;
    font-size: .93em;
    line-height: 1.6em;
    word-break: break-word;
    background: rgba(255, 255, 255, .4);
    span {
        margin-right: 1em;
        color: #B5B5B5;
        font-weight: bold;
    }
    a {
        color: gray;
        &:hover {
            font-weight: bold;
            color: #a3d2a3;
            text-decoration: underline;
        }
    }
    &:hover p .copy-path::after {
        content: "复制";
    }
    .post-url:hover {
        font-weight: normal;
    }
    .copy-path {
        margin-left: 1em;
        &:hover {
            color: gray;
            cursor: pointer;
        }
    }
}
```
- 第一段的toc-article指定了目录整个的背景色、边框色、倒角半径、各种间距以及最大的宽度。注意这里最好指定目录的最大宽度，我将其设为了28%，也就是文章正文那个框的宽度的28%，也可以设为一个固定的长度，比如在笔记本电脑上16em就是个不错的宽度，但为了能适配各种不同尺寸的屏幕，最好还是设置为百分比。如果不指定最大宽度，遇到比较长的标题时，生成的目录会非常难看。这个最大宽度的设置是我在网上其他添加目录的方法中没有见到的。
- 第二段的toc-title指的就是“文章目录”那四个字，这四个字要比其他字大一些，将其字号设为其他字的120%。
- 第三段的#toc.toc指定了目录列表的一些细节，将font-size设为0.9em会让目录的字比文章的字稍小一些。最后的.toc-child指定了二级目录的缩进量。
再次生成页面，应该已经可以显示比较美观的目录了。

	下面我就需要编辑每一篇需要添加目录的文章，在文章开头的front-matter中加入toc: true。

# 插入自定义页面
仿照Hexo官网，了解到单页面的添加方式。
```
\layout\plugins.swig

<div id="content-wrap">
  <div class="wrapper">
    <div class="inner">
      <header id="plugin-list-header">
        <h1 id="plugin-list-title">{{ page.title }}</h1>
        <input type="search" id="plugin-search-input" placeholder="Search">
        <div id="plugin-list-count">{{ site.data[page.data].length }} items</div>
      </header>
      <ul id="plugin-list">
        {% for plugin in _.sortBy(site.data[page.data], 'name') %}
          {{ partial('_partial/' + page.partial, {plugin: plugin}) }}
        {% endfor %}
      </ul>
    </div>
  </div>
</div>
<script>window.SEARCH_INDEX = {{ lunr_index(site.data[page.data]) }}</script>
```

```
layout\_partial\plugin.swig

<li class="plugin on">
  <a href="{{ plugin.link }}" class="plugin-name" target="_blank">{{ plugin.name }}</a>
  <p class="plugin-desc">{{ plugin.description }}</p>
  <div class="plugin-tag-list">
    {% for tag in plugin.tags %}
      <a href="#{{ tag }}" class="plugin-tag">{{ tag }}</a>
    {% endfor %}
  </div>
</li>
```

```
\layout\_partial\work.swig


<li class="plugin on">
  <div class="plugin-screenshot">
    <img src="{{ plugin.imgs }}" class="plugin-screenshot-img">
    {% if plugin.preview %}
    <a href="{{ plugin.preview }}" class="plugin-preview-link" target="_blank"><i class="fa fa-eye"></i></a>
    {% endif %}
  </div>
  <a href="{{ plugin.link }}" class="plugin-name" target="_blank">{{ plugin.name }}</a>
  <p class="plugin-desc">{{ plugin.description }}</p>
  <div class="plugin-tag-list">
    {% for tag in plugin.tags %}
      <a href="#{{ tag }}" class="plugin-tag">{{ tag }}</a>
    {% endfor %}
  </div>
</li>
```

```

引入样式文件
D:\Hexo\Hexos\themes\spfk\source\css\style.styl

@import "_partial/plugins"
```
## 修改样式
```
\layout\_partial\plugin.swig

#plugin-list-header
  clearfix()
  margin: 40px 0

#plugin-list-title
  font-family: font-title
  font-size: 36px
  font-weight: 300
  line-height: 1
  float: left

#plugin-list-count
  color: color-gray
  padding-top: 1em
  text-align: right
  @media mq-normal
    float: right
    line-height: 40px
    padding-top: 0
    padding-right: 15px

#plugin-search-input
  font-size: 16px
  font-family: inherit
  -webkit-appearance: none
  border: 1px solid color-border
  padding: 10px 10px
  width: 100%
  margin-top: 25px
  @media mq-normal
    float: right
    width: 50%
    margin-top: 0

#plugin-list
  margin: 40px -20px
  display: flex
  flex-flow: column
  @media mq-tablet
    flex-flow: row wrap

.plugin
  display: none
  padding: 20px
  @media mq-tablet
    flex: 0 0 50%
  @media mq-normal
    flex: 0 0 (100 / 3)%
  &.on
    display: block

.plugin-name
  font-family: font-title
  font-weight: bold
  color: color-link
  font-size: 20px
  text-decoration: none
  line-height: 1
  &:hover
    color: color-link-hover

.plugin-desc
  line-height: line-height
  margin: 1em 0

.plugin-tag-list
  clearfix()
  line-height: 1.3

.plugin-tag
  color: color-gray
  font-size: 0.9em
  text-decoration: none
  float: left
  margin-right: 10px
  &:hover
    color: color-link-hover
  &:before
    content: "#"

.plugin-screenshot
  margin-bottom: 15px
  position: relative
  padding-top: (10 / 16 * 100)% // 16:10 ratio
  height: 0
  overflow: hidden

.plugin-screenshot-img
  position: absolute
  top: 0
  left: 0
  width: 100%
  height: auto

.plugin-preview-link
  position: absolute
  top: 0
  left: 0
  width: 100%
  height: 100%
  background: rgba(0, 0, 0, 0.7)
  color: #fff
  text-align: center
  opacity: 0
  transition: 0.15s
  &:hover
    opacity: 1
    .fa
      opacity: 1
      transform: scale(1)
  .fa
    position: absolute
    top: 0
    left: 0
    bottom: 0
    right: 0
    margin: auto
    font-size: 50px
    width: @font-size
    height: @font-size
    opacity: 0
    transform: scale(6)
    transition: 0.2s
    transition-delay: 0.15s
```


# 自定义挂件
除了默认已提供的挂件外，你还可以自定义自己的小挂件，在hexo\themes\modernist\layout_widget\下，新建自己的ejs文件，如myWidget.ejs，然后在配置文件hexo\themes\modernist_config.yml中配置。
```
widgets:
  - myWidget
用上述方法可以添加新浪微博小挂件。

生成自己的微博组件。
添加hexo\themes\modernist\layout\_widget\weibo.ejs文件。
配置hexo\themes\modernist\_config.yml。
```
# Hexo语法高亮
查阅格式高亮代码，了解到本主题，通过特定的规律进行语法高亮！好像无法识别不同代码的语法高亮！
测试：
通过测试代码，查看后台代码逻辑，了解到可以识别Apache、C++、bash等，还有部分不可识别。那么这个主题用的是什么的语法高亮？
代码code，table-gutter-pre是代码前面的序号。class=”highlight apache”
```
source\css\_partial\highlight.styl

// https://github.com/luuman/hexo-theme-spfk

code-bgc = #002B36
code-tag = #F92672
code-attr = #A6E22E
code-word = #FFFFFF
code-value = #E6DB74
code-number = #9E90FF
code-keyword = #66D9EF
code-comment = #75715E
code-argument = #FD971F

$code-block
  background: code-bgc
  margin: 10px 0
  padding: 10px 10px
  overflow: auto
  color: #4C4C4C
  line-height: font-size * line-height
```
参考：
highlight.js：
Demo [https://highlightjs.org/static/demo/](https://highlightjs.org/static/demo/)
Solarized Dark
Atelier Sulphurpool Dark
文档：[http://highlightjs.readthedocs.org/en/latest/css-classes-reference.html](http://highlightjs.readthedocs.org/en/latest/css-classes-reference.html)
下载：[https://highlightjs.org/download/](https://highlightjs.org/download/)
# 首页添加loading效果

```
\layout\index.ejs

<link rel="stylesheet" href="css/loading-style.css">
<div id="loader-wrapper">
    <div id="loader"></div>
</div>

<%- partial('_partial/archive', {pagination: 2, index: true}) %>
<!-- loading -->
<script>window.jQuery || document.write('<script src="js/jquery-1.9.1.min.js"><\/script>')</script>
<script type="text/javascript">
    $(window).load(function() {                              // makes sure the whole site is loaded
        $('#loader').fadeOut();                              // will first fade out the loading animation
            $('#loader-wrapper').delay(350).fadeOut('slow'); // will fade out the white DIV that covers the website.
        $('body').delay(350).css({'overflow-y':'visible'});
    })
</script>

```
# LoadingBar页面顶部加载进度条
layout_partial\head.ejs
```
<!-- 加载特效 -->
<% if(theme.animate) { %>
 <script src="/js/pace.js"></script>
<link href="/css/pace/pace-theme-flash.css" rel="stylesheet" />
<% } %>
```
# Hexo插件


- https://swiftype.com/




```

```


# Buer博客中的图片视频类资源使用七牛云存储

## 七牛云存储

[七牛云](https://qiniu.com/)

### 图片水印接口

	?watermark/2/text/5Zu-54mH5p2l5rqQIGh0dHBzOi8vYnVlci53ZWJzaXRl/font/5a6L5L2T/fontsize/500/fill/IzAwMDAwMA==/dissolve/100/gravity/Center

# Hexo-Theme-Buer Debug

## Update Log

### 2016.6.20

* `[+]` 在文章页中添加上一篇和下一篇文章链接。
* `[^]` 修改 font-family 顺序，避免微软雅黑将单引号解析为全角。
* `[^]` 修复标签云算法中被除数为零的 bug。

### 2016.5.11 v2.0.1

* `[^]` 优化代码，将页面中的大段评论相关代码抽离出来，放入`comments.html`
* `[+]` 添加百度统计和Google分析代码，在`_config.yml`中配置相关参数即可
* `[+]` 更新文档，添加博客主题使用方法，便于上手
* `[+]` 添加了`favicon.ico`
* `[^]` 修复 bug，目录太长时，滚动到最底部时隐藏到footer下面。修复后长目录在滚动到底部时使用`position:absolute`
* `[^]` 修改目录区的滚动条样式（仅针对`webkit`内核浏览器）
* `[^]` 修改 demo 页中 disqus 评论区 a 标签的颜色 bug，修改 blockqoute 中 p 标签的 margin
* `[+]` 添加不蒜子计数功能，在footer上显示访问量
* `[+]` 添加回到顶部功能

### 2016.4.27 v2.0.0

* `[^]` 基于hexo重构了所有代码
* `[+]` 主页添加了摘要，在正文中使用4个换行符来分割，可在`_config.yml`中修改
* `[+]` 主页添加了近期文章、分类列表和标签云
* `[+]` 主页导航区做了视觉优化，阴影效果
* `[+]` 增加了归档、标签和分类页面
* `[+]` 增加了收藏页面
* `[+]` 评论插件可以选择 disqus 或 多说，直接在`_config.yml`中修改
* `[+]` 适配移动端
* `[+]` 页面滚动时，文章目录固定在右侧
* `[+]` 页面内容较少时，固定 footer 在页面底部
* `[^]` 使用 GitHub 风格的代码高亮写法，即\`\`\`的写法，去除`highlight.js`代码高亮插件的使用
* `[^]` 使用 Masonry 重写了 Demo 页中的瀑布流布局，响应式交互体验更好





