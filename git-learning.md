#  git的使用

## 一、上传代码到github

 ##### 步骤

`cd 文件名 `  : 进入该文件

`git init` :初始化

`git add .`  :将该文件夹下面的文件都添加进来，若要添加某个特定文件，将 . 换成文件名即可

`git add README.md`

`git commit -m "提交信息（备注）"`  

`git push -u origin master`  ：把本地仓库push到github上



`git status` :查询状态

 

#####  将github上的仓库克隆到本地

``` git Bash
  git clone http://github.com/Xvwenjun/.......git
```



#####  将本地仓库关联到github

``` git Bash
  git remote add origin git@ http://github.com/Xvwenjun/.......git
```



`git pull origin master`

` git push -u origin master`



## 二、下载代码

1、到github复制giturl

2、新建文件夹

3、git bash here

4、`git clone`





## 三、更新代码

###  1、本地代码没有修改过

直接使用   `git pull`  , 必须要本地代码没有修改过的情况。



### 2、本地代码有修改，多分支

`git checkout master` : 切换到master分支

`git pull` :  更新master分支

`git checkout isso` ：切换到自己的分支isso

`git merger master ` ：把master分支合并到自己的分支

 

### 3、本地代码有修改，只有master分支，直接覆盖本地代码

`git reset -- hard` : 重置索引和工作目录

`git pull` :  更新代码



### 4、本地代码有修改，直接覆盖远程仓库代码

`git push -- force origin isso `: 覆盖isso分支

`git push -- force origin master` :  覆盖主分支