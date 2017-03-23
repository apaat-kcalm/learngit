#远程仓库#
## 添加TA（先有本地库，再有origin）##
 ssh-keygen -t rsa -C "401671898@qq.com" 一路回车
添加SSH  id_rsa.pub
验证:ssh -T git@github.com
yes

### 环境准备 ###
- git remote add origin git@github.com:apaat-kcalm/learngit.git
远程库的名字就是origin

 **(第一次推送)**
- -git push -u origin master
加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，

###正文###

推送最新修改给分支

**本地提交之后（add，commit）**
**git push orign <分支名>**

##先创建远程库，然后，从远程库克隆##
命令：git clone/cd/ls
 git clone git@github.com:apaat-kcalm/HTMUAKTBT-.git
cd HTMUAKTBT-

ls  查看已有文件

#多人协作#
- 查看远程仓库：git remote
##流程##
- 从仓库克隆至本地：git clone git@github.com:apaat-kcalm/HTMUAKTBT-.git
- 新建本地分支+切换分支： git checkout -b dev origin/dev
-  添加+推送
	-  git add,
	-  git commit
	-  git push origin dev

> $ git add file1.txt
> $ git add file2.txt file3.txt
> $ git commit -m "add 3 files.

**ps: 推送失败**
- 因为远程分支比你的本地更新，需要先用git pull(抓取最新提交)试图合并；
- 如果合并有冲突，则解决冲突，并在本地提交；
- 没有冲突或者解决掉冲突后，再用git push origin 分支名 推送就能成功！

**ps: 如果git pull提示“no tracking information”，**

则说明本地分支和远程分支的链接关系没有创建，用命令git branch --set-upstream branch-name origin/branch-name。

###开源项目###
- 在其项目主页，folk
- 从自己账号下folk到本地
- pull request：推送修改给作者


