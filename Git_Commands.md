======Begin======

Step 1: Download repository from GitHub
`git clone https://xxx`

---------------------------------------------------

Step 2: Check status of modified files.
`git status` # Modified files are in red in this step

---------------------------------------------------

Step 3: Select files you want to operate.
`git add --all` #

---------------------------------------------------

Step 4: Check status of modified files again.
`git status` # Modified files are in green in this step

---------------------------------------------------

Step 5: Commit the changes in local PC with message.
`git commit -m "information"`

---------------------------------------------------

Step 6: Push the changes to GitHub.
`arc diff` # company requirment
`git push origin master` # You can set branch here

---------------------------------------------------

======Update======

Before following steps, check your branch:
`git branch` (you should be in 'develop' branch)
If not in 'develop' branch, run:
`git checkout develop`
If no 'develop' branch, create by:
`git branch develop`

--------------------------------------------------

Step 1: Every time you want to update, first check version.
`git log --oneline`
If the log are not the same, run:
`git pull origin develop`
And then check log again:
`git log --oneline`

--------------------------------------------------

Step 2: Repeat Step2-6 in 'Begin' section.
!! Notice: Step6 should be:
`git push origin develop`

---------------------------------------------------

### Give up modification
`git reset --hard`

======Merge branch======
1. `git fetch`
3. `git merge origin/develop` # origin means remote, so you are actually merge from remote

=====Renaming Git Branch======
1. `git checkout <old_name>`
2. `git branch -m <new_name>`
3. `git push origin --delete <old_name>`
4. `git push origin -u <new_name>`

======Delete a branch======
1. `git branch -d <branch_name>`
2. `git push -d <remote_name> <branch_name>`
