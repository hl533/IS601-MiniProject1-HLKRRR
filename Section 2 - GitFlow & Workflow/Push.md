# Push - 

>The `git push` command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo. It's the counterpart to `[git fetch](https://www.atlassian.com/git/tutorials/syncing/git-fetch)`, but whereas fetching imports commits to local branches, pushing exports commits to remote branches.
>
>Push the specified branch to <remote>, along with all of the necessary commits and internal objects. This creates a local branch in the destination repository. To prevent you from overwriting commits, Git won’t let you push when it results in a non-fast-forward merge in the destination repository.
>
>`git push` is most commonly used to publish an upload local changes to a central repository. After a local repository has been modified a push is executed to share the modifications with remote team members.

In the below diagrams, the local copy of the master has advanced past the remote/origin master. By using ```git push origin master```, the contributor is able to push the local changes to the remote master, and make them matching again.

![enter image description here](https://www.atlassian.com/dam/jcr:f148974e-7d4d-4c0e-bd31-8ac5467d1e6a/04.svg)

The command for Git push is:
```git push <targetbranch>```

In this project, we mostly did ```git push origin master``` and ```git push origin xxx-branch```.

[https://www.atlassian.com/git/tutorials/syncing/git-push](https://www.atlassian.com/git/tutorials/syncing/git-push)
