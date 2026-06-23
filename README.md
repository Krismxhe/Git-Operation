# Git-Operation
standard protocal to create/modify a github repo

## Git init repo
Initialize a GitHub repo
```
git init
```

Check the config of the GitHub repo
```
git config -l
```

Initialize username and Email
```
git config --global user.name "name"

git config user.email "name@example.com"
```

Add remote git repo
```
cd existing_repo
git remote add origin https://github.com/example.git
git pull https://github.com/example.git
git branch -M main
git push -uf origin main
```

Commit
```
git add .
git commit -m "message"
```

Push to an existing git repo
```
git push
```
Or
```
git push -f origin main
```
## Merge
The wrong order of push and pull operation will cause asynchronous conflict. We need to merge first.
```
git merge
```
```
git push
git pull
```
## Remove existing git info
Remove git directory
```
rm -rf .git
```

Clean the cache
```
git rm -rf --cached ./target_file
```


## Create a new local workspace, associate to a existed repo, create a new branch
```
1. 下载远程仓库到本地（创建新 Workspace）
```
git clone https://github.com/Krismxhe/Medical-Image-Segmentation-Baseline.git
```
2. 切换到项目根目录
```
cd Medical-Image-Segmentation-Baseline

```
3. 同步远程主分支的最新代码
```
git pull origin main

```
4. 创建并切换到全新的功能开发分支
```
git checkout -b feature-polarseg

```
5. [在此阶段进行代码编写/修改]
6. 将所有修改或新增的代码放入暂存区
```
git add . 

```
7. 提交代码到本地仓库，并记录清晰的 Commit 信息
```
git commit -m "feat: create a new branch for fundus polar seg"

```
8. 将 HTTPS 链接切换为更安全的 SSH 密钥链接
```
git remote set-url origin git@github.com:Krismxhe/Medical-Image-Segmentation-Baseline.git

```
9. 将本地新分支推送到 GitHub 远程仓库
```
git push origin feature-polarseg

Keep doing the original protocol.
