


This is a description which tell you how to use the github with some action

No.1 Create
Click the git bash in your computer
mkdir xxx(filename)              #build the new file
cd xxx(filename)                 #change the path
pwd                              #show the present file
'''
notice:文件不要用记事本编辑，用notepad++
'''

git init                         #the file change into a managed repository

git add xxx                      #add the file into storage
git  commit -m "xyz"             #submit into repository and do a description
'''
notice:add可以添加多个文件，commit可以一次全部提交
'''

No.2 Command
git status                       #look the repository present status 
git diff                         #look the file difference between now and before
git log                          #show the record of submit log
'''
notice:最近版本为head，上一版本为head^，上上版本为head^^，上一百个版本为head~100
'''
git reflog                       #show the recod of command 

git reset -- hard HEAD^          #repository return to the last version

cat xxx                          #show the content of file

git checkout -- xxx              #give up the modify for the workspace

git reset HEAD xxx  +  <git checkout -- xxx>
                                 #give up the modify for the storage
'''
如果已经提交到版本库，但还未推送到远程仓库，可使用版本追回
'''
git rm + <git commit>            #delete the file and do a explan

git cheekout -- xxx              #从版本库中还原文件
 
No.3 plant space
'''
本地客户端中，分为工作区，暂存区以及版本区
工作区就是一个目录下的空间，你可以创建本地文件，可以删除或添加内容
而暂存区和版本区存在于文件夹“.git”中，当你使用<git add>命令时，文件xxx被传入暂存区
当使用<git commit>命令时，文件xxx被提交至版本区

'''
No.4 remote repository
                                 #remote repository which is built in github 
git remote add origin git@github-----            
                                 #后面的是地址，前面的命令用于本地库与远程仓库的关联
git push -u origin master        #用来向远程库提交新修改的内容
'''
git remote ---的内容只有新创建远程仓库时，需要关联，若改仓库已经关联过
则第二次提交时，只需要<git push -u origin master>

