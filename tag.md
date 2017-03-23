#标签#
###操作：###
- 查看：git tag
- 查看tag信息：git show <tagname>

####新建：####
- git tag 名
-  git tag -a <标签名> -m "描述说明" commit-id
#### 补增标签####
 - commit-id
 ：git log --pretty=oneline --abbrev-commit
- git tag 名 commit-id
####[PGP签名](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/001376951758572072ce1dc172b4178b910d31bc7521ee4000)

####推送####
- 单个：git push origin <tagname>
- 一次性：git push origin --tags

##删除标签##
###本地###
git tag -d 标签名
###远程###
- 删本地
-  git push origin :refs/tags/<tagname>
