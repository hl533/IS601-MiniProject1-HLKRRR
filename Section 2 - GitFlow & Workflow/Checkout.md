# Checkout- 
>"In Git terms, a "checkout" is the act of switching between different versions of a target entity. The `git checkout` command operates upon three distinct entities: files, commits, and branches. In addition to the definition of "checkout" the phrase "checking out" is commonly used to imply the act of executing the `git checkout` command.
>
>The  `git checkout`  command lets you navigate between the branches created by  `git branch`. Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch. Think of it as a way to select which line of development you’re working on.
>
>It makes it ridiculously easy to try new experiments without the fear of destroying existing functionality, and it makes it possible to work on many unrelated features at the same time. In addition, branches also facilitate several collaborative workflows.
>
>The  `git checkout`  command may occasionally be confused with  `git clone`. The difference between the two commands is that clone works to fetch code from a remote repository, alternatively checkout works to switch between versions of code already on the local system.

In short, if your local project looks like this:

![Checkout](https://wac-cdn.atlassian.com/dam/jcr:389059a7-214c-46a3-bc52-7781b4730301/hero.svg?cdnVersion=612)
Then using ```git checkout <branchname>```will allow you to jump to any specific commit or branch in the history of the project and revert changes, merge branches, or any number of other functions.

[https://www.atlassian.com/git/tutorials/using-branches/git-checkout](https://www.atlassian.com/git/tutorials/using-branches/git-checkout)
