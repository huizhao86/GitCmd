# 1.进入要管理的文件夹  
cd <文件夹名>  
```cd c#```  
# 2.执行初始化命令  
```git init```  
# 3.管理文件夹内的文件状态  
```git status```  
# 4.管理指定文件  
```
git add <文件名>   
git add .
```  
# 5.个人信息配置，邮箱和用户名（一次即可）  
```  
git config --global user.email "hui_zhao86@hotmail.com"  
git config --global user.name "zhaohui"  
```  
# 6.生成版本  
```  
git commit -m '描述信息'  
```  
# 7.查看版本记录  
```  
git log  // 此处可能一直出现：，可以通过键盘q退出
```  
# 8.版本回滚  
```  
git reset --hard <版本号>  //类似于md5的一串数字，直接回滚到上一个版本状态  
```  
# 9.回滚后查看废弃的版本
```  
git reflog  
```  
# 10.其他命令  
```  
git checkout  //将修改后的文件会滚到上次一保存状态  
git reset head  //将暂存区文件会滚到修改状态  
git reset --mix <版本号>  //从版本库会滚到修改状态  
```  
# 11.分支  
```  
git branch <分支名>  //创建分支  
git checkout <分支名>  //切换分支
# 13.删除无用的分支，即bug分支合并到主分支后即无效了，可以删除
```  
# 12.合并分支，首先要切换到主分支，然后再去合并想要的分支，注意合并的顺序，即谁合并谁
```
git branch <主分支名>  //先切换到主分支
git merge <其他分支名>  //再合并其他分支
```
# 13.删除无用的分支，即bug分支合并到主分支后即无效了，可以删除
```
git branch -d <分支名称>  
```
# 14.重命名当前分支  
```  
git branch -m <分支名称>
```
# 15.克隆源代码仓库  
```  
git clone <仓库地址>  //此处测试了终端清屏快捷键command+k
```
# 16.给远程仓库起别名  
```  
git remote add <别名> <仓库地址>  //别名一般使用origin
```  
