# GitFlow & Workflow - 
Git is a tool that allows for collaborative and parallel work on a single project by many people. The branching workflow that is often used in large projects lets teams work on separate features and versions of a project, and allows contributors and managers to easily test versions, track history, find bugs, and in general, work collaboratively.

Here is an example diagram of what a GitFlow/Workflow might look like:

![GitFlow](https://nvie.com/img/git-model@2x.png)

### In this example, there are 5 different types of [branches](./Branch.md/). Let's break it down:
- **Master** - [Link](./Master%20Branch.md/)

The Master Branch (light blue) is the only version of the project that the public sees, and is generally very stable and is not often changed except during new releases, or if there are bugs that need to be urgently hotfixed.

- **Develop**

The Develop Branch (yellow) is where, naturally, where most of the development stems from. Any features developed in the Feature Branches or bug fixes from the Release or Hotfix branches will be pushed back to here. This will generally be the most up-to-date version of the project.

- **Feature**

The Feature Branches (pink) are created to work on specific discrete features of the project. A contributor or team of contributors can work on this branch, independently from other Feature Branches, and experiment and tinker without the fear of interrupting the work of other teams or the main project. Different Feature Branches can easily be [merged back](./Merge.md) into the Develop Branch at different points in time, when it comes time to get the project ready for release/deployment.

- **Release**

The Release Branch (green) is created to bugtest (no new features created here) the Develop Branch and prepare it for deployment to the public on the Master Branch. The Release Branch is tested in a suitable test environment, with bugfixes merged back to the Develop Branch as necessary. When testing is complete, the Release Branch is merged to both the Develop Branch and the Master/Deployment Branch.

- **Hotfix**

The Hotfix Branch (red) is used to fix issues not detected while testing the Release Branch, and that urgently need to be resolved, without waiting for the standard workflow. This branch is directly 'branched' off the Master, and when the hotfix is complete, is merged back to both the Master and Develop Branches.

[https://datasift.github.io/gitflow/IntroducingGitFlow.html](https://datasift.github.io/gitflow/IntroducingGitFlow.html)
