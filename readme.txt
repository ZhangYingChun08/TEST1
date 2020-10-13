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

<<<<<<< HEAD
10...测试 git diff --cached，克隆到本地新仓库后修改

1111....本地仓库离线修改提交
=======  git pull  从远程库下载到本地自动合并失败，需要人工处理冲突
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
<<<<<<< HEAD
<<<<<<< HEAD

-------新建临时 分支 issue-101 处理 BUG !!!  BUG 101
=======    提交远程失败，报告需要先获取远程更新(git pull)，获取更新自动合并失败，这里手动修改
>>>>>>> 2b76cd783533b32797f4471bd6932206c1b70920
>>>>>>> 032cfa0b6093d75903c6a50654ec44ca30586349
=======   2020/10/13 16:32 人工合并

<<<<<<< HEAD
-----------------------！！！！！！！！！！！！！！！！！！！！
-----在 dev 分支修改

---- dev 分支修改还未 staged
=======    通过 git cherry-pick 2b056ef 合并其他分支的修改，这里时自动合并失败，手动处理的
-------新建临时 分支 issue-101 处理 BUG !!!  BUG 101
>>>>>>> 2b056ef... fixed bug 101
>>>>>>> dev
