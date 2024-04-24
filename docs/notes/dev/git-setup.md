---
layout: default
title: Git Commands
parent: Software Development
grand_parent: Notes
---


## useful git commands

git is a version control system

## setup on new machine

First you need to generate SSH key. The name will be displayed in git when you commit a code.

```bash
ssh-keygen -t rsa -b 4096 -C "name"
```

press Enter for default settings.

Then setup global account.

```bash
git config --global user.name "username"
git config --global user.email "email"
```

## clone repository

Clonning is saving a copy of remote repository to local computer. Navigate to directory where all the source codes are located. Then run the following command. The repository address is available on website of the code (github or gitlab).

```bash
git clone git@gitlab.com:user/repository.git
```

## new branch

```bash
git checkout -b newLocalBranch
```


## push commits to a remote

```bash
git push remoteName branchName
```

by default the remoteName is origin in 99% of cases

## merge options

```bash
git checkout --ours -- <paths>
git checkout --theirs -- <paths>
```

## checkout specific file from another branch

```bash
git checkout branchName -- filePath
```

## discard uncommited changes

discard all the changes

```bash
git checkout -- .
```

discard only specific file

```bash
git checkout -- filePath
```
