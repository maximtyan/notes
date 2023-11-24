---
layout: default
title: Advice for PC Configuration
parent: Python Development
---

## Advice for PC configuration

Tips that can make code development little bit easier
and more efficient regardless of programing language, OS and your
experience.

## Make your username easy to type

Make it short, use small letters, use only latin symbols, avoid using
spaces or special symbols.

My username on any PC is **maxim** (5 symbols, no capital
letters, no spaces, no special symbols).

You will probably have to type your username in a system terminal quite
 often. Keeping it simple will save you time and your little finger.

Sometimes you need to type a directory path in a terminal. Some
terminals require quotes if the path contains space.

```cmd
cd ./username/
cd "./user name/"
```

Removing space from path name will save you some more time.

The same advice can be applied to any directory, file name, name of
your project and other names you will have to type often.

## file names and directories

Same advice can be applied to any file and directory name.
Try to keep it short, avoid unicode, spaces or other special symbols.

## Keep the source code closer to disc root

I recommend to keep all your development projects closer to disc root.
It will simplify navigation and allow to avoid errors with old programs.

I keep my development projects at:

```text
D:\src
```

Some old analysis programs often used in engineering have limitations
for the length of file path. For example XFOIL and AVL will not run if
the path length is longer than 40 symbols.

AVL cannot open this file:

```text
D:\my-study\classes\aircraft-design\design-code\avl-input-file.txt
```

But it will open this

```text
D:\src\design-code\avl-inp.txt
```
