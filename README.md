# MyImageHosting
Github+jsDelivr+PicGo 搭建的个人图床，这套方案完全免费 ，全程零成本，体验却一点也不差。

# 优势
- 免费！免费！免费！说三遍
- 快，实测图片国内访问速度非常快，足够日常使用
- 高效，能够一键批量处理图片上传存储

# 为何要搭建个人图床

轻松维护
- 平时我们将图片夹杂在文章、文档、公众号、博客当中，一般情况下这样似乎没有任何问题， 可试想一下若我们需要同时维护多份，不停地在不同渠道重复上传、编辑，图片也会散落各地，难以维护管理，这时候若有个统一的存储地方就可以很轻松维护。

- 提升页面访问速度
 过去我们将图片直接放到在线静态页面当中的话，在访问时需要等待全部资源加载，然而一般页面都是图片较大。当我们将图片分离后异步加载，再通过CDN加速，能够大幅提升页面的访问速度。

- 减少原页面服务器访问压力
由于访问图片的请求都经由图床/CDN，使得原来页面所在的服务器访问压力减少

# github充当云存储

[详见](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#github%E5%9B%BE%E5%BA%8A)

# [jsdelivr充当CDN](https://www.jsdelivr.com/?docs=gh)

eg
- 我的这个图床仓库地址是 https://github.com/buqiyuan/MyImageHosting
- 即cdn的地址为：https://cdn.jsdelivr.net/gh/buqiyuan/MyImageHosting
- 栗子：[https://cdn.jsdelivr.net/gh/buqiyuan/MyImageHosting/imgs/uni-chat/emojis/qq/0@2x.gif](https://cdn.jsdelivr.net/gh/buqiyuan/MyImageHosting/imgs/uni-chat/emojis/qq/0@2x.gif)

# PicGo充当图片git push工具

[https://github.com/Molunerfinn/PicGo](https://github.com/Molunerfinn/PicGo)

# 配置 PicGo

到达这一步我们已经得到：

- 图床仓库名
- 图床仓库对应的git分支
- github账号Token
- cdn地址

接下来打开PicGo这个工具分别填入以上内容，进行配置，注意选择github图床，具体可参照[PicGo官方文档](https://picgo.github.io/PicGo-Doc/zh/guide/config.html#github图床)
