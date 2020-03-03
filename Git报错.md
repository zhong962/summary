# Git学习中出现的报错及纠正
1. 在连接到远程仓库的操作时，输入`git remote add origin 地址`时，报错如图：
![img](https://img-blog.csdnimg.cn/20190310163241467.PNG)
这说明这个远程仓库地址已存在，这样就算成功了，如果还是要纠正，可以输入`git remote rm origin`
然后在输入连接远程仓库的命令即可；

2. 更多的错误是在将文件推送到GitHub时无法成功，后来发现是本地文件和GitHub的不同步，最开始输入`git push -u origin master`时,出现以下报错：
![img](https://upload-images.jianshu.io/upload_images/10229294-3ecc41ae759a4de2?imageMogr2/auto-orient/strip|imageView2/2/w/821/format/webp)                     
即README.md文件没有从GitHub同步到本地文件库里，一开始我试着从远程仓库里pull到本地文件，输入`git pull origin master`,结果还是无法成功，后来，请教了别人之后才解决了我的问题，即直接将远程仓库里的文件克隆到本地，输入命令`git clone 远程仓库地址`，然后就可以在本地看到克隆下来的文件，在进行操作就没有错误了！

3. 因为第一次使用GitHub，还不太懂怎么使用，最主要是在GitHub上直接修改或添加文件会导致文件不同步，所以以后要记得在本地库里编辑文件。

#### 可以参考以下网址：(https://www.jianshu.com/p/feb3a14c24ef)