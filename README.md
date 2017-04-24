# test
## 本仓库用于测试合作开发项目，谨慎删除

#### 当前项目内容：
* 17/04/24 DeclarationFromBot.html 打字机效果

***

#### 说明：
* 本地只能同时登录一个github账号

* [git] git fetch | git pull
	
  git fetch 拉取远程repo但不自动合并分支
  	-- git diff master origin/master
  	-- git merge origin/master
  
  git pull 拉取远程repo并自动合并分支

* error: failed to push some refs to 'https://github.com/ladxiaolong/test.gi
  hint: Updates were rejected because the remote contains work that you do
  hint: not have locally. This is usually caused by another repository pushi
  hint: to the same ref. You may want to first integrate the remote changes
  hint: (e.g., 'git pull ...') before pushing again.
	
	当远程repo已经更新， 而本地没有拉取合并新内容， 本地无法直接git push