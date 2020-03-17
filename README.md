# testasdasd

git push using script as below :

#! /bin/bash
# make folder and copy file
mkdir push_folder
echo "DIR where files were available"
read -p "input DIR : " DIR
cp -a $DIR push_folder
cd push_folder
git init
git add .
read -p "input commit message : " MES
git commit -m "$MES"
read -p "input repository : " repos
git remote add origin $repos
git push -u origin master

ps : only for first time push
