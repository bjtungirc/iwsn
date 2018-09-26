# github
git是版本控制软件，github是图形化管理git的网站。
# 安装
- windows下载exe双击下一步
- mac、linux一般自带
# 实操
- 创建一个github仓库
- 本地初始化项目，关联github仓库
- 本地提交，并推送
# 小结
```bash
# 将当前目录初始化为一个git仓库
git init 
# 将某个文件添加到暂存区
git add filename
# 将暂存区的内容提交到本地仓库
git commit -m "提交的注释"
# 将本地仓库推送到远程（github）仓库
git push origin master
# 查看提交日志
git log --graph
# 查看操作日志
git reflog
# 回滚版本
git reset --hard <版本号>
```
# 要求
能在本地创建git仓库，提交文件，回滚版本。  
能提交到github，能从github拉取。  
课后需要去完成的： 
- 深入理解git本地三个区：工作区、缓存区、本地仓库。
- git冲突时如何解决
- 灵活使用branch
# 作业：用github搭建静态博客
[作业1](../homework/work1.md)
