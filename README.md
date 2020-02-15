/*
以下是本主题的配置, 采用JSON格式
其中Name, Version, Author, AuthorUrl是必填项(注意首字大写)
你也可以定义其它的配置, 如FriendLinks, 在模板文件使用 $.themeInfo.FriendLinks来获取值

注意:
1) JSON语法严格, 键必须用双引号, 最后不得有空','来结尾
2) 以下配置不能包含任何注释, 不然解析会出错!

请在此解析所有配置
* Name 主题名
* Version 主题版本
* Author 主题的作者
* AuthorUrl 作者的博客链接或相关链接
* github github角标跳转
* Postend 文章结束标记，默认打开为trun
* copyright：文章结尾版权信息，默认打开为trun

* FriendLinks 友情链接

* gitalk 评论系统相关配置
  clientID clientID
  clientSecret clientSecret
  repo  用来存储评论的仓库名
  owner 管理员
  admin 谁可以初始化仓库，是个数组，一般填写管理员就行了
* music 音乐单页
    name	-	音频名称
    artist	-	音频艺术家
    url	-	音频链接
    cover	-	音频封面
    lrc	-	歌词详情
    theme	-	切换到此音频时的主题色，比上面的 theme 优先级高
*/
{
  "Name": "dllcn-simple-pebbles",
  "Version": "1.0",
  "Author": "myllcn.com",
  "AuthorUrl": "http://myllcn.com",
  "github": "https://github.com/KeiferJu",
  "Postend": true,
  "copyright": true,
  "FriendLinks": [
    {"Title": "我的官网", "Url": "http://myllcn.com"},
    {"Title": "我的博客", "Url": "http://blog.myllcn.com"},
    {"Title": "npm", "Url": "https://www.npmjs.com/~jkf19980216"},
    {"Title": "Github", "Url": "https://github.com/KeiferJu"}
  ],
  "gitalk": {
    "clientID": "b76c9107e35a12bee4f2",
    "clientSecret": "62d8dbc028003efa3e44c982f2d758cff743508d",
    "repo": "KeiferJu.github.io",
    "owner": "KeiferJu",
    "admin": ["KeiferJu"]
  },
  "music": [
    {"name":"RightNow","artist":"RightNow","url":"http://blog.myllcn.com/music/RightNow.mp3","cover":""},
    {"name":"怒放的生命","artist":"汪峰","url":"http://link.hhtjim.com/qq/001faIUs4M2zna.mp3","cover":""}
  ]
}
