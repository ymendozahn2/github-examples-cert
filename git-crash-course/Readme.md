## Cloning

We can clone 3 ways: HTTPS, SSH, Github CLI

Since we are using Github Codespaces, we are going to create a temp directory in out workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

## Git Hidden Folder

There is a hidden folder called .git which tells you that our project is a git repo.

If we wanted to create a git repo in a new project, we create the folder and then initialize that repo using `git init``

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add .


# makes changes to the readme.md file
git commit -a -m "add readme file"
```

## HTTPS

```sh
git clone https://github.com/ymendozahn2/github-examples-cert.git
cd github-examples-cert
```
> You'll need to generate a Personal Github Access Token (PAT)

https://github.com/settings/token

You will use the PAT as your password

## SSH

```ssh
                                                                                                                                                                    
```

## Commits

When we want to commit changes to the main, we can use
`git commit`, and it will open on the editor for writing 
comments to the commit.

```sh
git commit
```

Set the global editor for opening files
```sh
git config --global core.editor emacs
```
You can get files commited without opening the editor
```
git commit -m "the comment for the commit"
```
## Branches

List of branches
```
git branch 
```

create a new branch
```
git branch <branch-name> 
```

checkout the branch
```
git checkout <branch-name>
```

```
git push --set-upstream origin dev
```

## Remotes

we can add remotes via upstream when adding a branch

```
git remote add ...
git branch -u origin new-feature
```

## Stashing

```
git stash list
git stash
git stash save my-name
```

## Merging

## Add

When we want to stage changes for all files changes, we can use
`git add .``

## Reset

Reset command allows you to move staged changes to be unstaged.
This is useful if you want to clear the staged files.

## git status

Git status shows you what files will or will not be commited.

```
git status
```

## config

Whe you first install git on a machine, you are suppose to setup you name and email address.

```sh
git config --global user.name "Pedro Perez"
git config --global user.email "pedro.perez@example.com"
```

## log

git log will show the recent git commits to the git tree

```
git log
```

## Push

When we want to push a repo to our remote origin

```
git push
```