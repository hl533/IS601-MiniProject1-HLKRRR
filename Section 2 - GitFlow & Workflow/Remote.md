# Remote Add / Remove / Show
>The `git remote` command lets you create, view, and delete connections to other repositories. Remote connections are more like bookmarks rather than direct links into other repositories. Instead of providing real-time access to another repository, they serve as convenient names that can be used to reference a not-so-convenient URL.
>
>The `git remote` command is essentially an interface for managing a list of remote entries that are stored in the repository's `./.git/config` file.

Some simple commands that involve Git Remote:
- ```git remote show``` Lists all the remote repositories connected to the current local repository
- ```git remote add <http or ssh url of remote repository>```  Connects the current local repository to the specified remote repository
- ```git remote rm <name>``` Disconnects the current local repository to the specified remote repository, with the name being what is displayed in the ```git remote show``` command

[https://www.atlassian.com/git/tutorials/syncing](https://www.atlassian.com/git/tutorials/syncing)
