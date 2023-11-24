---
layout: default
title: Buttons
parent: Python Development
nav_order: 2
---


# useful git commands

git is a version control system

## setup on new machine

First you need to generate SSH key. The name will be displayed in git when you commit a code.

```git
ssh-keygen -t rsa -b 4096 -C "name"
```

press Enter for default settings.

Then setup global account.

```git
git config --global user.name "username"
git config --global user.email "email"
```

## clone repository

Clonning is saving a copy of remote repository to local computer. Navigate to directory where all the source codes are located. Then run the following command. The repository address is available on website of the code (github or gitlab).

```git
git clone git@gitlab.com:user/repository.git
```

## new branch

```git
git checkout -b newLocalBranch
```


## push commits to a remote

```git
git push remoteName branchName
```

by default the remoteName is origin in 99% of cases

## merge options

```git
git checkout --ours -- <paths>
git checkout --theirs -- <paths>
```

## checkout specific file from another branch

```git
git checkout branchName -- filePath
```

## discard uncommited changes

discard all the changes

```git
git checkout -- .
```

discard only specific file

```git
git checkout -- filePath
```
