git推送远程仓库报错

		git push -u origin master 报错：
	

	fatal: 'git@github.com/zejun_web' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
原因remote命令错误
 
	解决方法：
		remove添加在远程的origin
		git remote rm origin （之后再去推送即可）


git ssh配置无误但无法链接github仓库
	报错：Host Key Verification Failed
缺少文件 执行命令：
		ssh-keyscan -H github.com >> ~/.ssh/known_hosts
