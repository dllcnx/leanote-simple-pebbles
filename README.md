# leanote-simple-pebbles

[观看效果](http://note.myllcn.com/preview?themeId=5e40c662499442000d00007e)

根据官方主题市场生活的simple-pebbles进行修改，原主题字体大小等等都进行太大，总感觉不舒服，进行了样式微调。替换了官方disqus评论系统为gittalk，因为一些原因，Disqus国内无法使用，但是又懒得去翻，就用了基于git的gittalk。
添加了音乐单页。
所以此主题使用需要你处理两点。

1. 修改themem.json文件，来让页面尾部的链接都替换成你的。
2. 如果要启动gittalk评论，首先需要将你的博客设置评论选择Disqus方式，id随意，用不到了。然后在themem.json里面gitalk的对应位置填写你申请的github OAuth Apps相关信息。

![1](./images/screenshot.png)

![2](lib/gitalk.png)
```
* gitalk 评论系统相关配置
  clientID clientID
  clientSecret clientSecret
  repo  用来存储评论的仓库名
  owner 管理员
  admin 谁可以初始化仓库，是个数组，一般填写管理员就行了
  
  {
    ......
    
    "gitalk": {
      "clientID": "xxx",
      "clientSecret": "xxx",
      "repo": "xxx",
      "owner": "xxx",
      "admin": ["xxx"]
    }
  }
```
3. 如果要启用音乐单页，需要在你的博客设置里面添加一个单页，并将路由命名为music。然后可以在theme.json文件中添加自己想要的音乐。
![3](./lib/music1.png)
```
* music 音乐单页
    name	-	音频名称
    artist	-	音频艺术家
    url	-	音频链接
    cover	-	音频封面
    lrc	-	歌词详情
    theme	-	切换到此音频时的主题色，比上面的 theme 优先级高
{
  ......
  
  "music": [
    {"name":"RightNow","artist":"RightNow","url":"http://blog.myllcn.com/music/RightNow.mp3","cover":""}
  ]
}
```
