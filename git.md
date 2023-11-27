## GIT

#### Q1. How can you check your current git version? [R]

- [ ] git --v
- [x] git --version
- [ ] git --option
- [ ] git --current

[Reference](https://www.howtogeek.com/759319/how-to-check-and-update-your-git-version/)

#### Q2. What command lets you create a connection between a local and remote repository? [R]

- [ ] git remote add new
- [x] git remote add origin
- [ ] git remote new origin
- [ ] git remote origin

[Reference](https://stackoverflow.com/questions/20291731/how-to-connect-to-a-remote-git-repository)


#### Q3. Which of the following is true when you use the following command? [R]

`git add -A`

- [x] All new and updated files are staged
- [ ] Files are staged in alphabetical order.
- [ ] All new files are staged
- [ ] Only updated files are staged

[Reference](https://git-scm.com/docs/git-add)
[Reference](https://www.geeksforgeeks.org/difference-between-git-add-a-and-git-add/)

#### Q4. After you make changes to a local repository, you run the following command. What will this do? [R]

`git commit -a -m "Refactor code base"`

- [ ] Nothing, you can't use multiple options in the same command
- [ ] Adds all new files to the staging area
- [ ] Commits all new files with a message
- [x] Adds all modified files to the staging area, then commits them with a message

#### Q5. Where are files stored before they are committed to the local repository? [R]

- [ ] Saved files
- [ ] git documents
- [x] Staging area
- [ ] git cache

[Reference](https://www.geeksforgeeks.org/what-is-a-git-repository/)

#### Q6. What is GitHub? [R]

- [ ] version control
- [x] A hosting platform for Git repositories
- [ ] for keeping images
- [ ] for social networking

#### Q7. What files is this .gitignore programmed to leave out? [U]

```shell
#.swift
build/

*.txt
*.metadata
```

- [ ] All files with a .swift, .txt, or metadata file extension, as well as the entire build directory
- [ ] Only the build directory
- [x] All files in the build directory, as well as files ending with .txt or .metadata
- [ ] Only files with .swift and .txt extensions.

[Reference](https://git-scm.com/docs/gitignore)

A line starting with `#` serves as a comment. Hence `# .swift` does not do anything. See `man gitignore`.

#### Q8. What commands would you use to force an overwrite of your local files with the master branch? [U]

- [ ] ⠀

```bash
  git pull --all
  git reset --hard origin/master
```

- [ ] ⠀

```bash
  git pull -u origin master
  git reset --hard master
```

- [ ] ⠀

```bash
  git pull origin master
  git reset --hard origin/myCurrentBranch
```

- [x] ⠀

```bash
  git fetch --all
  git reset --hard origin/master
```

**Note**: - The command `pull` is `fetch` followed by either `merge` or `rebase` (in this case, `merge`). We don't want to merge. Merge would be an action to our **repository**. We just want to overwrite our **local files**.

#### Q9. What is the main issue with using git rebase when working with multiple developers? [U]

- [x] Rebase affects only your repository and creates a diff in the master branch.
- [ ] Rebase creates a temporary copy of the master branch in the remote repo.
- [ ] Rebase moves the HEAD of the remote master branch one commit forward.
- [ ] Rebase deletes all commit history for the new feature branch.

#### Q10. What is the difference between `git fetch` and `git pull` [U]

- [ ] `git fetch` creates a new branch off the master branch, while `git pull` creates a new branch off the local repository's master branch.
- [ ] `git pull` downloads new data from a remote repository without integrating it into local files, while `git fetch` updates the current HEAD branch with the latest changes from the remote server.
- [x] `git fetch` updates remote tracking branches with changes from a remote repository, while `git pull` updates remote tracking branches with changes from a remote repository and merges them into their corresponding local branches.
- [ ] `git fetch` downloads and merges data from the local repository, while `git pull` informs your colleagues you are about to make changes to the master branch.

#### Q11. What situation can occur when attempting to combine branches containing changes to the same piece of code? [U]

- [ ] lost code
- [ ] automatic override
- [ ] collisions
- [x] merge conflict

#### Q12. While modifying a file, you're unexpectedly assigned an urgent bug fix on another branch. How can you temporarily save your local work without committing? [A]

- [ ] This is not possible, as you cannot save locally without committing.
- [ ] Run git hold to save a local copy of what you're doing to return to later.
- [ ] Save your work with git local-cache.
- [x] Use git stash to save your work and come back later and reapply the stashed commit.

[Reference](https://git-scm.com/docs/git-stash)

#### Q13. After mistakenly staging a file named myFile to the index, how would you remove it from the index to exclude it from your next commit? [A]

- [ ] Use git reset HEAD^.
- [x] Use git reset myFile.txt.
- [ ] Use git -rm myFile.txt.
- [ ] Use git reset.

#### Q14. After modifying some existing files in a repository, you decide to discard the changes. What command can you use? [A]

- [ ] git restore
- [ ] git undo
- [ ] git clean
- [x] git checkout .

#### Q15. After starting to merge a feature branch into your master branch, you encounter a merge conflict and decide you do not want to perform the merge. How can you stop the merge and restore to the pre-merge state? [A]

- [ ] Use git restore -p.
- [ ] Use git merge -u.
- [x] Use git merge --abort.
- [ ] Use git merge --undo.

#### Q16. You have just completed rebasing your master branch and need to manually update the remote master, even though there is a merge conflict. How can you accomplish this? [A]

- [ ] `git push --overwrite`
- [ ] `git push --update`
- [ ] `git push --assert`
- [x] `git push --force-with-lease`

#### Q17. What command takes changes from the master branch on the remote repository origin and merges then to the local checked-out branch? [A]

- [ ] `git commit -u origin`
- [ ] `git checkout origin`
- [x] `git pull origin master`
- [ ] `git push origin master`

#### Q18. While pushing changes to a remote repository, you receive the following message. How do you resolve this issue? [A]

```bash
error: failed to push some refs to 'https://github.com/myrepo/simple.git'
hint: Updates were rejected because the remote contains work that you do not hint: not have locally.
```

- [ ] Use the --atomic option with the push command.
- [x] Execute a pull, then resolve any merge conflicts and execute another push.
- [ ] Execute a fetch, then execute another push.
- [ ] Use the --force option with the push command.

#### Q19. How can you exclude untracked files within the working directory from a Git repository? [A]

- [ ] You cannot exclude the files from the repository.
- [ ] Tag the files with excluded.
- [x] Add a pattern matching the files to the .gitignore file.
- [ ] Add the files to the omitted branch

[reference](https://git-scm.com/docs/gitignore)

#### Q20. After making a commit, you notice that you forgot to include changes to the doge.txt file. What command or commands would you use to add the changes to the commit? [A]

- [x] ⠀

```bash
  git add doge.txt
  git commit --amend --no-edit
```

- [ ] ⠀

```bash
  git commit --amend --no-edit
```

- [ ] ⠀

```bash
  git add doge.txt
  git commit --patch --no-edit
```

- [ ] ⠀

```bash
  git commit --patch --no-edit
```
