## current configuration and config files locations
```git config --list --show-origin```

## setup user and email
```git config --global user.name "Madalin Dogaru"```
```git config --global user.email "email@address.com"```

## initiate repository
```git init . ```

## add all file changes to the index
```git add . ```

## list all branches
```git branch```

## commit all changes to an existing branch
```git checkout existing-branch-name```

## create new branch and commit changes to it
```git checkout -b any-branch-name```

## push contents if the current branch has an upstream branch
```git push ```

## push contents if the current branch doesn't have an upstream branch
```git push --set-upstream origin branch-name```
