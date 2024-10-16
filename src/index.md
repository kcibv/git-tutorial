# Git Tutorial for non-programmers

Git is a free and open source distributed version control system designed to 
handle everything from small to very large projects with speed and efficiency. 
It is the most popular version control system among professional programmers, 
and this tutorial aims to making it understandable and usable by non-programmers.

Git can be used both from the command-line interface (a.k.a. `cmd` under windows) or
via a graphical user interface. This page describes the operations that Git can
execute, independently from the type of interface and refers to other pages for 
the CLI and GUI way of doing it.


## Let's get started: `init`

Say that you have a folder `MyProject` containing some files (or empty) and you want to start 
version-controlling it with git. To do that you ask git to run the `init` operation.

The `git init` operation creates a `.git` subfolder inside the `MyProject` folder, which will
hold all the git internal files. You don't need to be concerned about that folder; just don't
delet it, or git will lost all its memory about the version history of `MyProject`.

> Learn how to perform the `git init` operation via the 
> [CLI](cli.md#git-init-operation) or via the [GUI](gui.md#git-init-operation).


## Save your work: `commit`

We all make backups of our work so now and then: we take the folder containig our work
and we make a copy of it, namining it something like `MyProject_2024-10-14`. So, if anything
goes wrong with the files in our working directory `MyProject`, we can always restore
an older version of it.

In git terms, this is a *commit* operation (to commit = consign or record for preservation).
You run a `git commit` operation and git will make a copy of your working directory and
give it a name for you. You can commit as many versions of your working directory as you want.

> Notice that git commit takes a snapshot of your entire working directory, but it does
> it in a smart and disk-space-efficient way: just the minimum amount of information
> strictly necessary will be stored on disk.

We will visually represnt the working directory (WD) and its commits (git name for snapshot/backup) 
as shown in the following picture.

![commits](assets/img/commit.png)

> Learn how to perform the `git commit` operation via the 
> [CLI](cli.md#git-commit-operation) or via the [GUI](gui.md#git-commit-operation).


## Restore your work: `checkout`

*in progress ...*


## Try new ideas: `branch`

*in progress ...*


## Synchronize branches: `merge`

*in progress ...*


## Start cooperating on existing projects: `clone`

*in progress ...*


## Share your contributions: `push`

*in progress ...*


## Stay in sync: `pull`

*in progress ...*
