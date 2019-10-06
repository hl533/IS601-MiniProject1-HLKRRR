# Branch –

>“When you're working on a project, you're going to have a bunch of different features or ideas in progress at any given time – some of which are ready to go, and others which are not. Branching exists to help you manage this workflow.
>
>When you create a branch in your project, you're creating an environment where you can try out new ideas. Changes you make on a branch don't affect the master branch, so you're free to experiment and commit changes, safe in the knowledge that your branch won't be merged until it's ready to be reviewed by someone you're collaborating with.”

Branches exist so that teams can work and experiment on a project, without making changes to the “master,” which is considered the deployable or ”True” version of the project. Changes can then be merged back to the master branch or any other branch later, after review, either through pull requests on github or the ```git merge``` command.

The command for branching is: 
```git branch <newbranchname>```

[https://guides.github.com/introduction/flow/](https://guides.github.com/introduction/flow/)
