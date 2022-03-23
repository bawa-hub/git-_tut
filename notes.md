# 1. git basics

~ setup git on new project
git init
git add .
git commit -m "message"
git add remote <url> [optional]
git push origin master

~ cloning
git clone <url>
or
git clone <url> <target_directory>

~ status of files
git status
git status -s [short status]

~ view commit history
git log
git log -p [difference introduced in each commit]
git log --stat [abbreviated stats for each commit]
git log --pretty=oneline [with less or more information]

~ tagging

# git branching

git branch branch_1
git branch branch_2
git checkout branch_1 [switch to branch_1]
git merge branch_2 [merge branch_2 in branch_1]
