# 1 git创建

## 1.1

1.创建SSH Key。

在用户主目录（C:\Users\Administrator）下，看看有没有.ssh文件，如果有，再看文件下有没有`id_rsa`和`id_rsa.pub`这两个文件，如果已经有了，可直接到下一步。如果没有，打开Git Bash，输入命令，创建SSH Key

直接回车就哦了

## 1.2



![img](https://images2015.cnblogs.com/blog/1192146/201707/1192146-20170714173049337-699715656.png)

 1出现上图，就说创建成功啦，再去用户主目录里找到`.ssh`文件夹，里面有`id_rsa`和`id_rsa.pub`两个文件，这两个就是SSH Key的秘钥对，`id_rsa`是私钥，不能泄露，`id_rsa.pub`是公钥，可以公开。

 

2.接下来到GitHub上，打开“Account settings”--“SSH Keys”页面，然后点击“Add SSH Key”，填上Title（随意写），在Key文本框里粘贴 `id_rsa.pub`文件里的全部内容。

## 1.3

点“Add Key”，你就应该看到已经添加的Key，可以添加多个Key

![img](https://images2015.cnblogs.com/blog/1192146/201707/1192146-20170714174315025-1450935601.png)





## 1.4

验证是否成功，在git bash里输入下面的命令

如果初次设置的话，会出现如下界面，输入yes 同意即可

![img](https://images2015.cnblogs.com/blog/1192146/201707/1192146-20170714175422400-33988795.png)

## 1.5 .

下面开始设置username和email，因为github每次commit都会记录他们

## 1.6

5.接下来就是把本地仓库传到github上去，之前在GitHub上建好一个新的仓库是，跳转的页面，完全按照上面的只是操作就可以了。

 `$ git remote add origin git@github.com:flora0103/example.git    ``//关联一个远程库命令， git@github.com:flora0103/example.git   这个是自己远程库`

`git push -u origin master    ``//关联后,第一次推送master分支的所有内容命令，此后，每次本地提交后，就可以使用命令git push origin master推送最新修改`

## 1.7

![img](https://images2015.cnblogs.com/blog/1192146/201707/1192146-20170711180601197-948815634.jpg)

 