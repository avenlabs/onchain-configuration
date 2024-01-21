#### Fetch Data Github
```sh
git branch -m onlylayer ol-testnet
git fetch origin
git branch -u ol-testnet ol-testnet
git remote set-head origin -a
```

#### Add More Commit After Commit
```sh
git add . # or add file one by one
git commit --amend --no-edit
```

#### Change Message Commit 
```sh
git commit --amend # And follow instruction
```

#### Accidentally commit something in master that should be in the new branch!
```sh
git branch new-branch // delete last commit from master branch
git reset HEAD~ --hard
git checkout new-branch
```

#### Accidentally commit to the wrong branch!
```sh
git reset HEAD~ --soft
git stash
git checkout true-your-branch
git stash pop
git add .
git commit -m "message here";
```

#### Diff not work 
```sh
git diff --staged
```
