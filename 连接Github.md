***
### 生成RSA密钥
* 打开shell(git bash),`ssh-kengen -t rsa -c 'email'`,
* 在home目录找到*.ssh*文件夹，里面有**id_rsa 、id_rsa.pub**
两个文件
* 将公钥粘贴到github账户中的ssh密钥中：`github>>settings>>ssh Key`。
***
### Case 1:本地建好了仓库，同步到github
* 登录github,创建repository`repo`,根据提示，在shell中输入以下：  
`git remote add origin git@github.com:*username*/repo.git`  
`origin`:远程仓库名  
* 第一次push,参数u,后续可以省略  
`git push -u origin master`  
`master`:本地分支名  
* 打开github 查看
*** 
### Case 2:Github先创建，clone到本地
* 先在github上创建repository  
* 打开shell,进入欲存放repository的目录
* `git clone git@github.com/xxxx/xxx.git`
