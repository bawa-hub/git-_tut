## 1. git basics

```
~ setup git on new project
git init
git add .
git commit -m "message"
git add remote <url> [optional]
git push origin master
```

```
~ cloning
git clone <url>
git clone <url> <target_directory> [clone in target directory]
```

```
~ status of files
git status
git status -s [short status]
```

```
~ view commit history
git log
git log -p [difference introduced in each commit]
git log --stat [abbreviated stats for each commit]
git log --pretty=oneline [with less or more information]
```

```
~ tagging

<!-- Creating Tags -->
<!-- Git supports two types of tags: lightweight and annotated. -->
<!-- A lightweight tag is very much like a branch that doesn’t change — it’s just a pointer to a specific commit. -->

git tag [listing tags]
git tag -a v1.0 -m "message" [Creating an annotated tag]
git show <tag_name> [see tag data along with commit]
git push origin <tag_name> [By default, git push command doesn’t transfer tags to remote servers.]
git push origin --tags [push all tags at once]
git tag -d <tag_name> [delete a tag on local repo]
git push origin --delete <tag_name> [remove tag from remote server ]
git checkout <tag_name> [checking out tags]
```

```
~ git aliases
```

## 2. git branching

```
a. branching and merging
git branch branch_1 [creating branch]
git branch branch_2
git checkout branch_1 [switch to branch_1]
git merge branch_2 [merge branch_2 in branch_1]
git checkout -b <branch_name> [create and checkout branch]
git branch -d <branch_name> [delete a branch]

<!-- If you changed the same part of the same file differently in the two branches you’re merging, Git won’t be able to merge them cleanly.
you’ll get a merge conflict
 -->

git status [see which files are unmerged at any point after a merge conflict]

<!-- Git adds standard conflict-resolution markers to the files that have conflicts, so you can open them manually and resolve those conflicts.
After you’ve resolved each of these sections in each conflicted file, run git add on each file to mark it as resolved.-->

git mergetool [fires visual merge tool]
git status [to verify all conflicts are resolved]
git commit [if all conflicts are resolved]
```

```
b. branch management
git branch [list all branches]
git branch -v [last commit on each branches]
git branch --merged [merged branches]
git branch --no-merged [not merged till now]
git branch --move bad-branch-name good-branch-name [change branch name]
git push --set-upstream origin corrected-branch-name [change branch_name also on server]
```

```
c. remote branches
d. rebasing
```
