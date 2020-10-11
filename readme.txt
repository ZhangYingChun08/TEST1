1.This is git test.

2.Git is a version of the best controller.

3.......第一次修改...11111111111111111-----------测试修改

4......再次修改(删除！)

5......在新建的 分支  branchname_zyc1 修改   
新建git branch branchname；切换git checkout branchname
或者：git checkout -b branchname   ----新建并切换到分支

6.....从远程获取后，本地修改再签入（想删除...再次修改................）

7....加入新的仓库后，第一次修改（修改）

9...增加本行文本

13...第一次测试自动合并失败后（手动合并后），再次测试合并，这里是master分支修改

10...测试 git diff --cached，克隆到本地新仓库后修改

11...GIT升级到2.28版后，用  git switch  -c branch1  新建和切换分支

<<<<<<< HEAD
<<<<<<< HEAD
12...在master分支修改。
=======    修改，处理冲突！！！
12...在分支BRANCH1 修改
>>>>>>> branch1
=======    第二次冲突处理
12...在分支BRANCH1 修改

13...第一次测试自动合并失败后（手动合并后），再次测试合并，这里是 branch1 分支的第二次修改
>>>>>>> branch1

$ git log --graph --pretty=oneline --abbrev-commit
-------上面格式化显示提交日志
$ git branch -d branch1
------上面删除分支