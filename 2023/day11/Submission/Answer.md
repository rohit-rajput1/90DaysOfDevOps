# Day 11 Task: Advance Git & GitHub for DevOps Engineers: Part-2

## Git Stash:
Git stash is a command that allows you to **temporarily** save changes you have made in your working directory, without committing them.This is useful when you need to switch to a different branch to work on something else, but you don't want to commit the changes you've made in your current branch yet.

To use Git stash, you first create a new branch and make some changes to it. Then you can use the command git stash to save those changes. This will remove the changes from your working directory and record them in a new stash. You can apply these changes later. git stash list command shows the list of stashed changes.

You can also use git stash drop to delete a stash and git stash clear to delete all the stashes.

## Cherry-pick:
**Git cherry-pick** is a command that allows you to select specific commits from one branch and apply them to another. This can be useful when you want to selectively apply changes that were made in one branch to another.

To use git cherry-pick, you first create two new branches and make some commits to them. Then you use git cherry-pick <commit_hash> command to select the specific commits from one branch and apply them to the other.

## Resolving Conflicts:
Conflicts can occur when you merge or rebase branches that have diverged, and you need to manually resolve the conflicts before git can proceed with the merge/rebase.
git status command shows the files that have conflicts, git diff command shows the difference between the conflicting versions and git add command is used to add the resolved files.

---
# Task-01 
- Create a new branch and make some changes to it.

![branch change](https://user-images.githubusercontent.com/76991475/226160020-76815895-8e96-428b-9bae-35af81b57bf9.png)

- Use `git stash` to save the changes without committing them.

![1](https://user-images.githubusercontent.com/76991475/226159900-bc0f0074-ebe3-4ee8-af47-36bc920213eb.png)

![git stash](https://user-images.githubusercontent.com/76991475/226159908-6a02672c-9754-475a-94ba-18a250666cf7.png)

- Use git `stash pop` to bring the changes back and apply them on top of the new commits

![git stash pop](https://user-images.githubusercontent.com/76991475/226159916-cdceb80b-e79f-40ac-a9b0-04edeb92106a.png)

- Use git `stash push` to delete all the thing which are in stash.

![git stash push](https://user-images.githubusercontent.com/76991475/226159921-b16dad58-fb1f-40a3-94d2-9f863997313d.png)

---

# Task-02
- In `version01.txt` of development branch add below lines after `“This is the bug fix in development branch”` that you added in Day10 and reverted to this commit.
- **Line2**>> `"After bug fixing, this is the new feature with minor alteration”`
Commit this with message `“Added feature2.1 in development branch”`

![2](https://user-images.githubusercontent.com/76991475/226169673-01793fd6-48ad-4386-890e-b658b5084bde.png)

- **Line3**>> This is the advancement of previous feature.
Commit this with message `“Added feature2.2 in development branch”`

![3](https://user-images.githubusercontent.com/76991475/226169677-83a99cb2-5921-4718-bdae-ca906a1b3a88.png)

- **Line4**>> Feature 2 is completed and ready for release.
Commit this with message `“Feature2 completed”`
- Line4>> Feature 2 is completed and ready for release

![4](https://user-images.githubusercontent.com/76991475/226169872-330fb92d-01e1-4830-8e4d-a7ef05d07552.png)

---

# Task-03
- In Production branch Cherry pick Commit `“Added feature2.2 in development branch”` and added below lines in it:

![Screenshot from 2023-03-19 16-22-26](https://user-images.githubusercontent.com/76991475/226170852-d64f5ccb-f2f5-42df-90fd-104a29b54eb0.png)

**Commit**: Optimized the feature.

---