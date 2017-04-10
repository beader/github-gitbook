# Github-Gitbook

gitbook是一个用node写的命令行工具，可以把markdown变成漂亮的html书本。你可以用git来进行版本控制，把文章内容push到github的master分支，把生成html文件push到github的gh-pages分支。这样就可以通过github来访问你的书本。但往往，build, deploy的过程会比较繁琐，如果好久不操作，可能会忘记这些命令。

gitbook同时是一个网站，他们提供一项服务，可以直接让我们在网页上一个很棒的markdown编辑器下写文章，点save之后，会自动把html托管在gitbook的网站上，非常非常方便，不需要记忆任何git相关的命令。但是gitbook网站的访问速度比github慢很多。

有没有两全其美的方法？

既然大家都是用git来管理版本，中间设置个双向同步，gitbook编辑器更新的内容，会自动同步到github上，本地提交push到github的内容，会自动同步到gitbook上。这样我们既可以使用gitbook的编辑器，又可以使用本地的编辑器。同时设置一个travis-ci，自动把github上master分支build成html页面同时push到github的gh-pages分支下。这样一来，网页同时也被托管到了github上。

* 该项目在gitbook上的链接 [https://www.gitbook.com/read/book/beader/github-gitbook](https://www.gitbook.com/read/book/beader/github-gitbook)
* 该项目在github上的链接 [beader.github.io/github-gitbook](beader.github.io/github-gitbook)



