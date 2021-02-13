# Yilia-qure 简约清新主题
================
## PC端
![2021-02-13100122](https://cdn.jsdelivr.net/gh/Anyway521/blogpic2@main/image/2021-02-13100122.png)

简约优雅的个人博客，移动端，适配pad，请访问 [我的博客](https://anyway521.gitee.io/) 查看效果。  
Powered by [yilia](http://litten.me/)

# 主题配置
## 安装
克隆代码
``` yml
git clone https://github.com/Anyway521/yilia-qure
```
把`yilia-qure`放到博客的`theme`目录里，并且在博客根目录的`_config.yml`作修改`theme: yilia-qure`

文件放置好后别忘记： `npm install` 一下，安装主题需要的依赖

## 配置文件
主题配置文件`_config.yml`大致内容如下：
``` yml
# Header
menu:
  主页: '/'
  #留言: '/MessageBoard/'
  归档: '/archives/'
  # 分类: '/categories/'
  #关于: '/about/'

# SubNav
subnav:
  csdn: '#'
  bilibili: '#'
  #weibo: "#"
  #zhihu: "#"
  #weixin: '#'
  #jianshu: "#"
  #douban: "#"
  #segmentfault: "#"
  github: '#'
  #acfun: "#"
  #mail: '#'
  qq: '#'
  #facebook: "#"
  #google: "#"
  #twitter: "#"
  #linkedin: "#"
  rss: '/atom.xml'

# 是否需要修改 root 路径
# 如果您的网站存放在子目录中，例如 http://yoursite.com/blog，
# 请将您的 url 设为 http://yoursite.com/blog 并把 root 设为 /blog/。
root:
# Content

# 文章太长，截断按钮文字，直接在文章里加入<!--more-->就可以注释掉这里
excerpt_link:   
# 文章卡片右下角常驻链接，不需要请设置为false
show_all_link: '展开全文'
# 数学公式
mathjax: false
# 是否在新窗口打开链接
open_in_new: true
fancybox: true

# 打赏
# 打赏type设定：0-关闭打赏； 1-文章对应的md文件里有reward:true属性，才有打赏； 2-所有文章均有打赏
reward_type: 1
# 打赏wording
reward_wording: '创作不易，感谢支持！'
# 支付宝二维码图片地址，跟你设置头像的方式一样。比如：/img/alipay.jpg
alipay: ''
# 微信二维码图片地址
weixin: ''


## 版权声明
copyright: 
    copyright_type: 1      # 0:关闭  1，copyright: true则开启 2，全都开启
    licensee_url: https://creativecommons.org/licenses/by-nc-sa/4.0/          # 当前应用的版权协议地址。
    licensee_name: '知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议'  # 版权协议的名称
    licensee_ename: 'CC BY-NC-SA 4.0'                                        #版权协议的英文名称
    licensee_img: https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png      # 版权协议的Logo


# 目录设定：0-不显示目录； 1-文章对应的md文件里有toc:true属性，才有目录； 2-所有文章均显示目录
toc: 1
# 标号隐藏：true:隐藏生成目录自带的标号 fasle:不隐藏，默认使用系统带的标号
toc_hide_index: true
# 目录为空时的提示
toc_empty_wording: '目录，不存在的…'

# 是否有快速回到顶部的按钮
top: true

# Miscellaneous 百度统计和谷歌统计
baidu_tongji: 
#google_analytics: ''

#网站图标，icon格式
favicon: '/img/timg.ico'

# 头像旋转
Rotate: false

# 你的头像url
avatar: '/img/me.jpg'

#是否开启分享，如果不需要建议不要开启
share_jia: true

# Counting words字数统计，看个人需要是否开启
word_count: true
 
# 文章类型，在上面word_count: true的前提下可以进行开启
# 具体类型在对应的md文件开头的 article_type属性进行定义。原创：article_type:0 ，，转载：article_type:1 :
article_type: true

#评论：只保留1.giteement 2.gitalk
#不需要使用某项，直接设置值为false，或注释掉

#1、giteement码云评论系统
giteement:
  enable: true  # 是否启用码云
  redirect_uri: https://anyway521.gitee.io/   # 回调地址
  oauth_uri: https://cors-anywhere.herokuapp.com/https://gitee.com/oauth/token  # 授权地址，不能更改
  giteeID: anyway521  # 码云账号英文名
  repo: comment     # 存储评论的 repo
  client_id: '0516788fddee56be44b3b4e8dd8d090500c7dc44e2077ecb1baec5f17a3263db'           #client ID
  client_secret: '48b25a6de68548079c7f237e14346d3f0609aef1626b72d15826b4062b4be430'       #client secret


#2、gitalk
gitalk:
  enable: false #用来做启用判断可以不用
  githubID: Anyway521
  repo: 'comments'
  # 存储博客评论的仓库地址，可以是存储博客的仓库
  ClientID: ''
  ClientSecret: ''
  adminUser: Anyway521
  distractionFreeMode: true

# 样式定制 - 一般不需要修改，除非有很强的定制欲望…
style:
  # 头像上面的背景颜色
  # header: '#00BFFF'
  # 右滑板块背景渐变色
  slider: 'linear-gradient(200deg,#e7eefc,#54c8ff)'

# slider的设置
slider:
  # 是否默认展开tags板块
  showTags: true

# MarkDown文件下载地址,如：http://md.xxwhite.com，以后会写文章教怎么上传原文，不会请留空
mdhost:

#pangu.js 用于自动加空格
pangu: true

# 智能菜单
# 如不需要，将该对应项置为false
# 比如
#smart_menu:
#  friends: false
smart_menu:
  innerArchive: '所有文章 '
  friends: '友链 '
  aboutme: '关于我'

friends:
  Git中文参考文档: 'https://git-reference.readthedocs.io/zh_CN/latest/'
  Hexo参考文档: 'https://hexo.io/docs/'
  MarkDown中文文档: 'https://markdown-zh.readthedocs.io/en/latest/'

#在这里添加任何配置，都加在“aboutme”的上面，否则会出问题
aboutme: <br>Yilia-qure<br><br>一个清新简约的主题<br><br>
```

