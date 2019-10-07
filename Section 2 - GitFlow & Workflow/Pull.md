# Pull - 

>The `git pull` command is used to fetch and download content from a remote repository and immediately update the local repository to match that content. Merging remote upstream changes into your local repository is a common task in Git-based collaboration work flows. The `git pull` command is actually a combination of two other commands, `[git fetch](https://www.atlassian.com/git/tutorials/syncing/git-fetch)` followed by `[git merge](https://www.atlassian.com/git/tutorials/using-branches/git-merge)`. In the first stage of operation `git pull` will execute a `git fetch` scoped to the local branch that `HEAD` is pointed at. Once the content is downloaded, `git pull` will enter a merge workflow. A new merge commit will be-created and `HEAD` updated to point at the new commit.

There are 2 common ways to do git pulls. Both the ways will start like the below diagram:

![Before the Pull](https://www.atlassian.com/dam/jcr:00d011ed-03dc-440f-afc5-9b13d5e14fbf/bubble%20diagram-01.svg)

1. The standard ```git pull```, which is essentially a ```git fetch``` immediately followed by a ```git merge```. It takes all the previously untracked commits in the origin (A, B, C) and pulls them into a new commit (H), that becomes the new head in the local branch.

![Regular Git Pull](https://www.atlassian.com/dam/jcr:b3a663dc-1985-40df-b0a5-c6bcbacd71af/bubble%20diagram-02.svg)

2. The other way, using ```git pull --rebase origin```, pulls the untracked commits (A, B, C) and adds them to the existing history in the local repo, and makes the local commit history a single linear one.

![enter image description here](https://www.atlassian.com/dam/jcr:3949703c-5db2-44c9-8383-3ebc51832b4d/bubble%20diagram-03.svg)

[https://www.atlassian.com/git/tutorials/syncing/git-pull](https://www.atlassian.com/git/tutorials/syncing/git-pull)
