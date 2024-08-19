# Git-Operation
standard protocal to create/modify a github repo

# Git init repo
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
git config --global user.name "Krismxhe"

git config user.email "hmxian2022@hotmail.com"
```

Add remote git repo
```
cd existing_repo
git remote add origin https://github.com/Krismxhe/DiffDR.git
git branch -M main
git pull
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
