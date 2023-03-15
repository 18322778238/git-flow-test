1. 什么是开源？
   开源即开放源代码，不仅提供程序而且提供程序源代码，而且代码是公开的。特点是任何人都可以去查看，修改和使用开源代码！
2. 什么是开源许可协议？
   常见的5种开源协议：1. B5D  2.（Apache Licence 2.0） 3.GPL  4.LGPL   5.MIT
3. 远程仓库的两种访问方式：
   第一种：HTTPS: 零配置，在每一次访问仓库的时候，需要重复的输入Github的账号和密码才能访问成功
   第二种：SSH：需要进行额外的配置，每次访问仓库的时候，不需要重复输入Github的账号和密码
4. 当第二次向仓库提交新的代码指令为   git push
5. 检测Github的ssh key是否配置成功：
   打开Git Bash 输入 ssh -T git@github.com
   输入yes 命令执行成功 出现Hi username！证明SSH key配置成功
6. 基于SSH将本地仓库上传到GitHub
   操作和使用HTTPS相同 唯一的区别是把更换了连接方式
7. git clone + 远程仓库的地址 将远程仓库克隆到本地
8. git branch 查看当前Git仓库的所有分支  默认情况下  分支前面有*号表示当前所处的分支
9. git branch + 分支名称 基于当前分支  创建一个新的分支  这个命令指挥创建一个新的分支不会自动切换到新分支里
10. git checkout + 分支名称  切换到指定的分支
   git checkout -b + 分支名称  创建新的分支 并且切换到新分支上
11. 合并分支
    首先切换到master分支 git checkout master
    其次在master分支上运行git merge命令 将所需要合并的分支合并到 master分支上  git merge + 分支名称
12. 删除分支  当把功能分支合并到master分支后 可以执行对应的命令来删除功能分支
    git branch -d + 分支名称  需要删除对应分支时，不能再当前的分支上
13. 将本地分支推送到远程仓库
    git push -u + 远程仓库的别名 本地分支名称：远程分支名称
    放不需要给本地分支重新命名时可以省略冒号以及后面的名字
    只有第一次推送分支的时候需要带一个 -u参数  之后可以直接使用git push推送代码
14. 查看远程仓库的所有分支列表
    git remote show + 远程仓库的名称（origin）    
15. 跟踪分支
    git checkout +  远程分支的名称
    git checjout -b 本地分支名称 远程仓库的名称/远程分支的名称
16. 拉取远程分支的最新的代码  git pull
17. 删除远程分支
    git push 远程仓库名称 --delete 远程分支名称

