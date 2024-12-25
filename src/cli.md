# Use Git via the Command-Line interface

This page will show how to perform the main git operations using the
git Command-Line Interface (CLI). For an explanation of what each
command does, see [this article](./index.md) insted.

> If you don't have the git CLI installed on your machine yet, you 
> can download it from the [git website](https://git-scm.com/downloadd).


## git init operation
> For a description of this operation see the [main tutorial](index.md).

To initialize a new git repository with the git CLI, from the command-line
shell, first create a new project directory (say `my-project`) and enter
it. 

![create-dir](assets/img/cli-init-1.png)

From within the `git-tutorial` folder, run the `git init` command.

![git-init](assets/img/cli-init-2.png)

This command creates a `.git` sub-directory in the `my-project` directory.


## git commit operation
> For a description of this operation see the [main tutorial](index.md).

In order to have some changes to commit, let's create two new files named 
`file1.txt` and `file2.txt`, let's write some text in them and let's save 
them.

You can visualize the current changes by using the `git status` command.

![git-status](assets/img/cli-commit-1.png)

Git has correctly detected that, compared to the initial status (empty
directory) there are two new files. 

Say that this is a version of our project that we want to commit; first 
of all we need to tell git which changes we want to commit and which not: 
for example you may want to commit only file1.txt or only file2.txt. You
do that by adding the changes you want to commit to a virtual bucket
named *staging area*, using the `git add` command. In this case we will
add all the changes to the staging area.

![git-status](assets/img/cli-commit-2.png)

If we run the `git status` command again, we see that the status has
changed: the two files are not in the *Untracked* status anymore, but
they are now under *Changes to be commited*.

![git-status](assets/img/cli-commit-3.png)

Now we can finally commit the changes and we do it using the
`git commit` command, following by a message that describes the
commit.

![git-status](assets/img/cli-commit-4.png)

If you run the `git statu` command again, git will tell you that
there have been made no changes since the last commit.

![git-status](assets/img/cli-commit-5.png)

You can repeat this as many times as you want. Let's apply some changes
and commit them. Let's modify the content of `file2.txt` and add another
file named `file3.txt`. After doing than, the status will be as follows:

![git-status](assets/img/cli-commit-6.png)

Again git has detected the changes correctly: 1 file added and 1 file
changed! Let's just stage and commit these changes.

![git-status](assets/img/cli-commit-7.png)

If you want to list all the commits stored so far, you can do so by
entering the `git log` command.

![git-status](assets/img/cli-commit-8.png)

As you can see, git has automatically assigned a unique name to each of
the two commits:

- The first commit is called `207d0da62d84f512bc043bd15fda01d37e3c8f25`
- The second commit is called `578184144f5aa00646f57f64518a08779f16d9f0`


## git checkout operation
> For a description of this operation see the [main tutorial](index.md).

So far we have initialized a git project and commited two sets of 
changes. Our project folder is now identical to the second commit. If
you want to go back to the first commit, you can use the `git checkout`
command.


## git branch operations
> For a description of this operation see the [main tutorial](index.md).
*in progress ...*

## git merge operation
> For a description of this operation see the [main tutorial](index.md).
*in progress ...*

## git clone operation
> For a description of this operation see the [main tutorial](index.md).
*in progress ...*

## git push operation
> For a description of this operation see the [main tutorial](index.md).
*in progress ...*

## git pull operation
> For a description of this operation see the [main tutorial](index.md).
*in progress ...*
