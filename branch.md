#创建和合并分支
##——可自动合并
$ pwd
/c/Users/Administrator/learnnote-git

- 查看分支：git branch

- 创建分支：git branch dev
- 切换分支 git checkout dev
- 创建+切换分支：git checkout -b dev
###add,commit之后
- 合并某分支到当前分支：git merge dev
- 删除分支：git branch -d dev

##——冲突，手动更改（MASTER主分支）
Automatic merge failed; fix conflicts and then commit the result.



用到的命令：
- $ git log --graph --pretty=oneline --abbrev-commit 查看分支合并情况
-  cat hh 查看文件内容
-  add,commit


![](./_image/2017-02-06-14-27-43.jpg)




#分支管理
##看不出来曾经做过合并
- Fast forward模式
##合并后的历史有分支
- --no-ff
表示禁用Fast forward：git merge --no-ff -m "merge with no-ff" dev
#强制删除（没有被合并过的分支）
git branch -D <name>

#多人协作
