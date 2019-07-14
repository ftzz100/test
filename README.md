创建一个github项目仓库之后，要将本地文件上传到github的操作方法：    
（此处用的是macbook）  
打开终端进入项目文件夹Test  
> cd Test  

创建说明文件  
```shell
echo "# test" >> README.md  
```

初始化，此命令会在当前目录下创建一个.git 
```shell
git init
```

将项目的文件添加到仓库中  
```shell
git add README.md
```

将add的文件commit到仓库  
```shell
git commit -m "first commit"
```

将本地的仓库关联到github上  
```shell
git remote add origin https://github.com/ftzz100/test.git
```

上传代码到github远程仓库  
```shell
git push -u origin master
```
然后会要求输入Username和Password，即输入github的账号和密码

下次再更新代码的时候就只用  
```shell
git add .  
git commint -m "注释说明"  
git push  
```
