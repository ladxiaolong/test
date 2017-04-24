# test
## 本仓库用于测试合作开发项目，谨慎删除

#### 当前项目内容：
* 17/04/24 DeclarationFromBot.html 打字机效果

***

#### 说明：
* 本地只能同时登录一个github账号

* [git] git fetch | git pull
	
  1\git fetch 拉取远程repo但不自动合并分支
  	(1)先用git fetch拉取远程repo最新内容  
  	
  		git fetch将会取得后面所用的origin/master的内容
  	(2)-- git diff master origin/master  
  	
  		在shell中查看当前分支与远程repo分支的冲突  
  	(3.1)-- git commit -a -m "annotation"  
  	
  		error: Your local changes to the following files would be   		
  		overwritten by merge:  
        README.md  
		Please commit your changes or stash them before you merge.  
		
		合并冲突之前，本地代码需要先commit到版本库， 
		因为git merge会覆盖工作区冲突文档内容  
  	(3.2)-- git merge origin/master  
  	
  		手动合并冲突代码   
  		此命令会自动把远程仓库代码和本地代码放在同一个文件下  
  		<<< HEAD  
  			// 本地当前分支版本库最新内容(具体版本由HEAD指向)  
  		===========  
  			// 远程仓库内容  
  		>>> origin/master  
  	(4) -- git commit -a -m "annotation"  
  		-- git push origin master  
  		手动合并冲突后，再次add并commit到版本库, 最后push  
  
  git pull 拉取远程repo并自动合并分支

* error: failed to push some refs to 'https://github.com/ladxiaolong/test.gi  
  hint: Updates were rejected because the remote contains work that you do  
  hint: not have locally. This is usually caused by another repository pushi  
  hint: to the same ref. You may want to first integrate the remote changes  
  hint: (e.g., 'git pull ...') before pushing again.  
	
	报错： 当远程repo已经更新， 而本地没有拉取合并新内容， 本地无法直接git push  


