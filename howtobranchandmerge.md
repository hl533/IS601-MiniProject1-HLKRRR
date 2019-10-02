# download a repository on GitHub.com to our machine
git clone https://github.com/hl533/IS601-MiniProject1-HLKRRR.git

# change into the `IS601-MiniProject1-HLKRRR` directory
cd 'IS601-MiniProject1-HLKRRR'/

# create a new branch to store any new changes
git branch my-branch

# switch to that branch (line of development)
git checkout my-branch

# make changes, for example, edit `file1.md` and `file2.md` using the text editor

# stage the changed files
git add file1.md file2.md

# take a snapshot of the staging area (anything that's been added)
git commit -m "my snapshot"

# push changes to github
git push --set-upstream origin my-branch

# merge branch to master (remember that git merge moves the specified branch to the current branch that's checked-out)
# First we run git checkout master to change the active branch back to master. Then we run the command git merge new-branch to merge the new feature into the master branch. Note that git merge merges the specified branch into the currently active branch
git checkout master
git merge my-branch
