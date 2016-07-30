


This is a description which tell you how to use the github with some action

No.1 Create
Click the git bash in your computer
mkdir xxx(filename)              #build the new file
cd xxx(filename)                 #change the path
pwd                              #show the present file
#notice:文件不要用记事本编辑，用notepad++

git init                         #the file change into a managed repository

git add xxx                      #add the file into storage
git  commit -m "xyz"             #submit into repository and do a description
#notice:add可以添加多个文件，commit可以一次全部提交

No.2 Command
git status                       #look the repository present status 
git diff                         #look the file difference between now and before
git log                          #show the record of submit log
#notice:最近版本为head，上一版本为head^，上上版本为head^^，上一百个版本为head~100
git reflog                       #show the recod of command 

git reset -- hard HEAD^          #repository return to the last version

cat xxx                          #show the content of file