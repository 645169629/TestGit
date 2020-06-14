## Git Learning

`git add <file>` ：添加至暂存区

`git commit -m "description"`：提交至工作区

`git status`：查看当前状态

`git diff`：查看文件改动

`git log`：查看提交(commit)的记录

`git log --pretty=oneline`

HEAD表示当前版本

`git reset --hard HEAD^`：回退到上个版本

`git reset --hard HEAD~100`：回退到上100个版本

`git reset --hard commit_id`：回到某个版本

`git rerflog`：记录每次命令

`git checkout -- file`：丢弃某个文件工作区的修改（回到最近一次git commit 或git add的状态）

`git reset HEAD <file>`：把暂存区的修改撤销掉

`git rm <file>`：用于从版本库删除某个文件

- ```
  $ git rm test.txt
  rm 'test.txt'
  
  $ git commit -m "remove test.txt"
  [master d46f35e] remove test.txt
  1 file changed, 1 deletion(-)
  delete mode 100644 test.txt
  ```

`git push  origin master`：本地内容推送到远程仓库（第一次推送加上-u参数）